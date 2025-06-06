# AI Security Posture Management (AI-SPM) Platform

A comprehensive enterprise-grade security platform designed to manage, monitor, and secure AI/ML assets throughout their lifecycle. The platform provides real-time threat detection, vulnerability management, compliance monitoring, and governance controls for AI systems.

## Features

### 🛡️ Core Security Capabilities
- **AI Asset Discovery & Inventory**: Automated discovery and cataloging of AI models, datasets, pipelines, and endpoints
- **Vulnerability Management**: Continuous security scanning with risk assessment and remediation tracking
- **Real-time Threat Monitoring**: 24/7 monitoring with anomaly detection and automated alerting
- **Security Incident Response**: Centralized incident management with workflow automation

### 📊 Compliance & Governance
- **Multi-Framework Compliance**: Support for NIST AI RMF, GDPR, SOC 2, ISO 27001
- **Automated Assessments**: Continuous compliance monitoring with scoring and reporting
- **Policy Management**: Centralized governance policies with enforcement capabilities
- **Audit Trail**: Comprehensive logging of all system activities and user actions

### 📈 Analytics & Reporting
- **Security Dashboard**: Real-time metrics, trend analysis, and executive reporting
- **Risk Analytics**: Advanced risk scoring and predictive threat modeling
- **Compliance Reporting**: Automated generation of compliance reports and certifications
- **Custom Dashboards**: Role-based views with personalized security insights

### 🔗 Third-Party Integrations
- **Wiz Security Platform**: Native integration for importing cloud security data
  - Automated asset discovery from cloud environments
  - Vulnerability and security alert synchronization
  - Compliance findings and risk factor mapping
  - Real-time data synchronization with configurable filters
- **API-First Design**: RESTful APIs for custom integrations
- **Webhook Support**: Real-time notifications for external systems

### 👥 Enterprise Features
- **Role-Based Access Control**: Granular permissions for different user roles and departments
- **Multi-Tenant Support**: Isolated environments for different business units
- **Integration Ready**: APIs for third-party security tools and enterprise systems
- **Scalable Architecture**: Designed for enterprise-scale deployments

## Technology Stack

### Frontend
- **React 18** - Modern component-based UI framework
- **TypeScript** - Type-safe development with enhanced developer experience
- **Tailwind CSS** - Utility-first styling with responsive design
- **Shadcn/UI** - Production-ready component library
- **TanStack Query** - Powerful data synchronization and caching
- **React Hook Form** - Performant forms with validation
- **Recharts** - Interactive data visualization

### Backend
- **Node.js** - High-performance JavaScript runtime
- **Express.js** - Fast, unopinionated web framework
- **TypeScript** - End-to-end type safety
- **Passport.js** - Comprehensive authentication strategies
- **Drizzle ORM** - Type-safe database operations
- **PostgreSQL** - Enterprise-grade relational database
- **Zod** - Runtime type validation and parsing

## Project Structure

```
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   │   ├── charts/     # Data visualization components
│   │   │   ├── layout/     # Layout components (sidebar, header)
│   │   │   └── ui/         # Base UI components (shadcn)
│   │   ├── hooks/          # Custom React hooks
│   │   │   ├── use-auth.tsx      # Authentication context
│   │   │   ├── use-toast.ts      # Toast notifications
│   │   │   └── use-mobile.tsx    # Mobile detection
│   │   ├── lib/            # Utility libraries
│   │   │   ├── queryClient.ts    # API client configuration
│   │   │   ├── utils.ts          # Common utilities
│   │   │   └── protected-route.tsx # Route protection
│   │   ├── pages/          # Application pages
│   │   │   ├── dashboard.tsx     # Main dashboard
│   │   │   ├── ai-assets.tsx     # Asset management
│   │   │   ├── vulnerabilities.tsx # Vulnerability tracking
│   │   │   ├── compliance.tsx    # Compliance management
│   │   │   ├── monitoring.tsx    # Real-time monitoring
│   │   │   └── auth-page.tsx     # Authentication
│   │   └── types/          # TypeScript type definitions
├── server/                 # Backend Express application
│   ├── auth.ts            # Authentication middleware
│   ├── db.ts              # Database connection
│   ├── routes.ts          # API route definitions
│   ├── storage.ts         # Data access layer
│   ├── index.ts           # Server entry point
│   └── vite.ts            # Development server setup
├── shared/                # Shared code between client/server
│   └── schema.ts          # Database schema and validation
├── ARCHITECTURE.md        # Detailed system architecture
└── package.json           # Dependencies and scripts
```

## Database Schema

### Core Entities

**Users**: User accounts with role-based permissions
- Roles: Security Analyst, AI/ML Engineer, Compliance Officer, CISO
- Attributes: credentials, profile information, department assignment

**AI Assets**: Comprehensive asset inventory
- Types: Models, Datasets, Pipelines, Endpoints
- Environments: Development, Staging, Production
- Metadata: ownership, dependencies, risk levels, compliance status

**Vulnerabilities**: Security findings and remediation tracking
- Severity levels: Critical, High, Medium, Low
- Status tracking: Open, In Progress, Resolved, False Positive
- Assignment and escalation workflows

**Security Alerts**: Real-time threat notifications
- Incident categorization and prioritization
- Automated response triggers
- Integration with external security tools

**Compliance Frameworks**: Regulatory and standards compliance
- Framework definitions: NIST AI RMF, GDPR, SOC 2, ISO 27001
- Assessment templates and scoring criteria
- Automated compliance monitoring

**Audit Logs**: Comprehensive activity tracking
- User actions and system events
- Data access and modification logs
- Compliance audit trails

## API Reference

### Authentication Endpoints
```
POST /api/register        # User registration
POST /api/login          # User authentication
POST /api/logout         # Session termination
GET  /api/user           # Current user information
```

### AI Asset Management
```
GET    /api/ai-assets              # List all assets (with filtering)
POST   /api/ai-assets              # Create new asset
GET    /api/ai-assets/:id          # Get asset details
PUT    /api/ai-assets/:id          # Update asset
DELETE /api/ai-assets/:id          # Delete asset
GET    /api/ai-assets/owner/:owner # Get assets by owner
```

### Vulnerability Management
```
GET  /api/vulnerabilities           # List vulnerabilities (with filtering)
POST /api/vulnerabilities          # Report new vulnerability
GET  /api/vulnerabilities/:id      # Get vulnerability details
PUT  /api/vulnerabilities/:id      # Update vulnerability status
GET  /api/vulnerabilities/stats    # Get vulnerability statistics
GET  /api/vulnerabilities/asset/:id # Get vulnerabilities for asset
```

### Security Monitoring
```
GET  /api/security-alerts          # List security alerts
POST /api/security-alerts          # Create security alert
PUT  /api/security-alerts/:id      # Update alert status
GET  /api/security-alerts/recent   # Get recent alerts
```

### Compliance Management
```
GET  /api/compliance/frameworks        # List compliance frameworks
POST /api/compliance/frameworks        # Create framework
GET  /api/compliance/assessments       # List assessments
POST /api/compliance/assessments       # Create assessment
GET  /api/compliance/overview          # Compliance dashboard data
```

### Dashboard & Analytics
```
GET  /api/dashboard/metrics         # Dashboard statistics
GET  /api/audit-logs               # System audit logs
```

### Wiz Integration Endpoints
```
GET  /api/integrations/wiz/status              # Check Wiz integration status
POST /api/integrations/wiz/sync                # Full sync (assets, vulns, alerts)
POST /api/integrations/wiz/sync-assets         # Sync only assets
POST /api/integrations/wiz/sync-vulnerabilities # Sync only vulnerabilities  
POST /api/integrations/wiz/sync-alerts         # Sync only security alerts
```

## Installation & Setup

### Prerequisites
- Node.js 18+ 
- PostgreSQL 13+
- npm or yarn package manager

### Environment Configuration
Create a `.env` file with the following variables:
```bash
# Database Configuration
DATABASE_URL=postgresql://username:password@localhost:5432/ai_spm
PGHOST=localhost
PGPORT=5432
PGUSER=your_db_user
PGPASSWORD=your_db_password
PGDATABASE=ai_spm

# Authentication
SESSION_SECRET=your_session_secret_key

# Application
NODE_ENV=development
PORT=5000

# Wiz Integration (Optional)
WIZ_CLIENT_ID=your_wiz_client_id
WIZ_CLIENT_SECRET=your_wiz_client_secret
WIZ_AUDIENCE=beyond-api
```

### Installation Steps

1. **Clone and Install Dependencies**
```bash
git clone <repository-url>
cd ai-spm-platform
npm install
```

2. **Database Setup**
```bash
# Create PostgreSQL database
createdb ai_spm

# Push database schema
npm run db:push
```

3. **Start Development Server**
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

### Production Deployment

1. **Build Application**
```bash
npm run build
```

2. **Start Production Server**
```bash
npm start
```

### AWS Deployment using CloudFormation

This project includes a CloudFormation template (`cloudformation.yaml`) to automate the deployment of the entire application stack on AWS.

**Overview:**

The CloudFormation template provisions the following major resources:
- A new VPC with public and private subnets, NAT Gateways, and an Internet Gateway.
- An Amazon RDS PostgreSQL database instance (private).
- An Amazon ECR repository to store your application's Docker image.
- An Amazon ECS cluster with a Fargate service to run the Node.js backend application.
- An Amazon S3 bucket to host the static frontend assets.
- An Amazon CloudFront distribution to serve both frontend assets (from S3 via OAC) and API requests (routed to an Application Load Balancer).
- An Application Load Balancer (ALB) to distribute traffic to the ECS backend.
- Necessary IAM roles, security groups, and AWS Secrets Manager entries for credentials.

**Prerequisites:**

1.  **AWS Account & CLI:** An AWS account and the AWS CLI installed and configured with appropriate permissions to create the resources mentioned above.
2.  **Docker:** Docker installed locally to build the application image. (Or a CI/CD system that can build Docker images).
3.  **Node.js & npm/yarn:** Required to build the application assets locally before deployment (`npm run build`).
4.  **jq (optional but recommended):** For easier parsing of AWS CLI JSON outputs.

**Deployment Steps:**

**Step 1: Build Application Assets and Docker Image**

First, build your application's frontend and backend assets, and then build the Docker image using the provided `Dockerfile`.

```bash
# 1. Install dependencies (if not already done)
npm install

# 2. Build the application (creates ./dist directory with backend and ./dist/public for frontend)
npm run build

# 3. Build the Docker image (replace 'your-app-image-name' with your desired image name)
docker build -t your-app-image-name:latest .
```

**Step 2: Push Docker Image to Amazon ECR**

The CloudFormation stack will create an ECR repository. You'll need to push your image there.

*   **If deploying for the first time:** You might need to deploy a minimal version of the stack first to create the ECR repository, or create it manually with the expected name (`<stack-name>/app-repository`).
    Alternatively, you can use the AWS console or CLI to create the ECR repository named `your-stack-name/app-repository` (where `your-stack-name` is what you will name your CloudFormation stack) before the first full deployment.

*   **To get the ECR repository URI after it's created by CloudFormation:**
    (Note: It's recommended to add `ECRRepositoryUri` to the `Outputs` section of `cloudformation.yaml` for easier retrieval.)
    ```bash
    aws ecr describe-repositories --repository-names "<your-stack-name>/app-repository" --query "repositories[0].repositoryUri" --output text
    ```
    (Replace `<your-stack-name>` with the name you'll give your CloudFormation stack). Let this be `ECR_REPOSITORY_URI`.

*   **Tag and Push the image:**
    ```bash
    # Login to ECR (replace <aws_account_id> and <aws_region>)
    aws ecr get-login-password --region <aws_region> | docker login --username AWS --password-stdin <aws_account_id>.dkr.ecr.<aws_region>.amazonaws.com

    # Tag your local image
    docker tag your-app-image-name:latest ${ECR_REPOSITORY_URI}:latest
    # Example: docker tag your-app-image-name:latest 123456789012.dkr.ecr.us-east-1.amazonaws.com/my-ai-spm-stack/app-repository:latest

    # Push the image
    docker push ${ECR_REPOSITORY_URI}:latest
    ```
    Make sure the tag you push (e.g., `latest`) matches the `DockerImageTag` parameter you'll use for the CloudFormation stack.

**Step 3: Deploy Frontend Assets to S3**

The CloudFormation stack also creates an S3 bucket for your frontend assets.

*   **To get the S3 bucket name after it's created by CloudFormation:**
    The bucket name is constructed as `<stack-name>-frontend-assets-<aws_account_id>-<aws_region>`.
    (Note: It's recommended to add `S3FrontendBucketName` to the `Outputs` section of `cloudformation.yaml` for easier retrieval.)
    You can also find it in the CloudFormation stack outputs if defined, or via the AWS console.

*   **Upload assets:**
    The frontend assets are in the `./dist/public/` directory after `npm run build`.
    ```bash
    aws s3 sync ./dist/public/ s3://<your-s3-bucket-name>/ --delete
    ```
    (Replace `<your-s3-bucket-name>` with the actual bucket name).

**Step 4: Deploy the CloudFormation Stack**

Now, deploy the main CloudFormation stack using the `cloudformation.yaml` file.

```bash
aws cloudformation deploy \
  --template-file cloudformation.yaml \
  --stack-name <your-stack-name> \
  --capabilities CAPABILITY_IAM CAPABILITY_NAMED_IAM \
  --parameter-overrides \
    DBPassword=<your-secure-database-password> \
    DockerImageTag=latest \
    # WizClientId=<your-wiz-client-id> (Optional) \
    # WizClientSecret=<your-wiz-client-secret> (Optional) \
    # SSLCertificateArn=<arn-of-your-acm-ssl-certificate> (Optional, for HTTPS on custom domain) \
  --region <aws_region>
```

**Key Parameters:**
*   `DBPassword`: A strong password for the RDS database master user.
*   `DockerImageTag`: The tag of the Docker image you pushed to ECR (e.g., `latest`).
*   `WizClientId` (Optional): Your Wiz Client ID if using the Wiz integration.
*   `WizClientSecret` (Optional): Your Wiz Client Secret.
*   `SSLCertificateArn` (Optional): If you have a custom domain and want HTTPS, provide the ARN of an ACM SSL certificate. For CloudFront with a custom domain, the certificate must be in `us-east-1`. The ALB, also using this parameter, requires a certificate in its own region. Ensure your certificate strategy aligns with this.

**Step 5: Accessing Your Application**

Once the stack is successfully deployed:
1.  Navigate to the AWS CloudFormation console, select your stack, and go to the "Outputs" tab.
2.  You should find an output for `CloudFrontURL` (or similar). This is the main URL for your application.
    (Note: The `Outputs` section in `cloudformation.yaml` must be populated with `CloudFrontURL`, `ECRRepositoryUri`, `S3FrontendBucketName` etc., for easy access.)

**Updating the Stack:**

To update the application:
1.  Re-build your Docker image and push it to ECR with a new tag or overwrite the existing tag (e.g., `latest`).
2.  Re-deploy frontend assets to S3 if they have changed.
3.  Re-run the `aws cloudformation deploy` command. If you only changed the `DockerImageTag` or application code (requiring a new image/S3 assets), you might not need to change other parameters. CloudFormation will update the ECS service to pull the new image.

**Deleting the Stack:**

To remove all resources created by the template:
```bash
aws cloudformation delete-stack --stack-name <your-stack-name> --region <aws_region>
```
**Note:** S3 buckets might not be deleted if they contain objects. You may need to empty the S3 bucket first. Similarly, ECR repositories with images might require manual cleanup if not set to auto-delete on stack deletion (not default). The RDS instance has a `DeletionPolicy` which you might want to set to `Delete` for non-production environments to avoid manual snapshot cleanup or costs.

## Usage Guide

### Initial Setup

1. **Access the Application**: Navigate to the application URL
2. **Create Admin Account**: Register the first user (will have admin privileges)
3. **Configure Organization**: Set up departments and user roles
4. **Import AI Assets**: Begin asset discovery and inventory

### User Roles & Permissions

**Security Analyst**
- Monitor vulnerabilities and security alerts
- Investigate security incidents
- Generate security reports

**AI/ML Engineer** 
- Manage AI assets and deployments
- Monitor model performance and behavior
- Implement security recommendations

**Compliance Officer**
- Oversee compliance assessments
- Generate compliance reports
- Manage governance policies

**CISO (Chief Information Security Officer)**
- Executive dashboard access
- Organization-wide security oversight
- Strategic security planning

### Key Workflows

**Asset Onboarding**
1. Navigate to AI Assets section
2. Click "Add New Asset"
3. Complete asset registration form
4. Assign ownership and environment
5. Configure monitoring settings

**Vulnerability Management**
1. Review vulnerability dashboard
2. Assign vulnerabilities to team members
3. Track remediation progress
4. Validate fixes and close tickets

**Compliance Monitoring**
1. Select compliance framework
2. Configure assessment parameters
3. Run automated compliance scans
4. Review results and generate reports

## Security Features

### Authentication & Authorization
- Session-based authentication with secure session management
- Role-based access control (RBAC) with granular permissions
- Multi-factor authentication support (extensible)
- Account lockout protection against brute force attacks

### Data Protection
- Password hashing using scrypt with salt
- SQL injection prevention via parameterized queries
- Cross-site scripting (XSS) protection
- Cross-site request forgery (CSRF) protection
- Input validation and sanitization

### Audit & Compliance
- Comprehensive audit logging of all user actions
- Data retention policies for compliance requirements
- Encrypted data storage for sensitive information
- Regular security assessments and vulnerability scanning

## Monitoring & Observability

### Application Monitoring
- Real-time application performance metrics
- Database query performance monitoring
- Error tracking and alerting
- User activity analytics

### Security Monitoring
- Failed authentication attempt tracking
- Suspicious activity detection
- Automated security alert generation
- Integration with SIEM systems

### Health Checks
- Application health endpoints
- Database connectivity monitoring
- Service dependency checks
- Automated failover capabilities

## Troubleshooting

### Common Issues

**Database Connection Errors**
- Verify PostgreSQL service is running
- Check database connection credentials
- Ensure database exists and is accessible

**Authentication Problems**
- Clear browser cache and cookies
- Verify session store configuration
- Check user credentials and account status

**Performance Issues**
- Monitor database query performance
- Check memory and CPU usage
- Review application logs for errors

### Support & Maintenance

**Log Files**
- Application logs: `logs/app.log`
- Error logs: `logs/error.log`
- Audit logs: Database audit_logs table

**Database Maintenance**
```bash
# Backup database
pg_dump ai_spm > backup.sql

# Restore database
psql ai_spm < backup.sql

# Update database schema
npm run db:push
```

## Contributing

### Development Guidelines
- Follow TypeScript best practices
- Implement comprehensive error handling
- Write unit and integration tests
- Document API changes and new features

## Wiz Integration Guide

### Overview

The AI-SPM platform includes native integration with Wiz security platform for automated import of cloud security data including assets, vulnerabilities, and security alerts.

### Setting Up Wiz Integration

#### 1. Obtain Wiz API Credentials

Contact your Wiz administrator to create API credentials:
- Navigate to Wiz console > Settings > Service Accounts
- Create a new service account with appropriate permissions
- Note down the Client ID and Client Secret

#### 2. Configure Environment Variables

Add the following to your `.env` file:
```bash
WIZ_CLIENT_ID=your_wiz_client_id
WIZ_CLIENT_SECRET=your_wiz_client_secret
WIZ_AUDIENCE=beyond-api
```

#### 3. Verify Integration Status

Check integration status via API:
```bash
curl -X GET "http://localhost:5000/api/integrations/wiz/status" \
  -H "Authorization: Bearer YOUR_SESSION_TOKEN"
```

### Using Wiz Integration

#### Full Data Sync

Sync all data types (assets, vulnerabilities, alerts):
```bash
curl -X POST "http://localhost:5000/api/integrations/wiz/sync" \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer YOUR_SESSION_TOKEN" \
  -d '{
    "assetFilters": {
      "cloudPlatform": "AWS",
      "limit": 100
    },
    "vulnFilters": {
      "severity": ["CRITICAL", "HIGH"],
      "limit": 50
    },
    "alertFilters": {
      "severity": ["CRITICAL", "HIGH"],
      "limit": 25
    }
  }'
```

#### Asset-Only Sync

Import cloud assets from Wiz:
```bash
curl -X POST "http://localhost:5000/api/integrations/wiz/sync-assets" \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer YOUR_SESSION_TOKEN" \
  -d '{
    "cloudPlatform": "Azure",
    "subscriptionId": "your-subscription-id",
    "limit": 200
  }'
```

#### Vulnerability Sync

Import security vulnerabilities:
```bash
curl -X POST "http://localhost:5000/api/integrations/wiz/sync-vulnerabilities" \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer YOUR_SESSION_TOKEN" \
  -d '{
    "severity": ["CRITICAL", "HIGH", "MEDIUM"],
    "status": ["OPEN", "IN_PROGRESS"],
    "limit": 100
  }'
```

### Data Mapping

#### Asset Transformation
- **Wiz Asset Types** → **AI-SPM Asset Types**
  - MachineLearningModel → model
  - Dataset → dataset
  - APIGateway → api
  - Pipeline → pipeline
  - Container → model (default)
  - Function → api (default)

#### Risk Level Mapping
- **Critical/High Risk Factors** → critical
- **Medium Risk Factors** → medium  
- **Low/No Risk Factors** → low

#### Status Mapping
- **RUNNING** → active (production environment)
- **STOPPED/TERMINATED** → inactive (development environment)

### Automated Sync Workflows

#### Scheduled Sync (Recommended)

Set up automated sync using cron jobs or task schedulers:

```bash
# Daily full sync at 2 AM
0 2 * * * curl -X POST "http://localhost:5000/api/integrations/wiz/sync" \
  -H "Authorization: Bearer YOUR_TOKEN" \
  -d '{"assetFilters":{"limit":1000}}'

# Hourly vulnerability sync
0 * * * * curl -X POST "http://localhost:5000/api/integrations/wiz/sync-vulnerabilities" \
  -H "Authorization: Bearer YOUR_TOKEN" \
  -d '{"severity":["CRITICAL","HIGH"],"limit":100}'
```

#### Integration Monitoring

Monitor sync results and handle errors:
```javascript
// Example response from sync operation
{
  "message": "Wiz sync completed successfully",
  "result": {
    "assets": {
      "imported": 45,
      "updated": 12,
      "errors": []
    },
    "vulnerabilities": {
      "imported": 23,
      "updated": 8,
      "errors": ["Failed to sync vulnerability CVE-2023-1234: Asset not found"]
    },
    "alerts": {
      "imported": 15,
      "updated": 3,
      "errors": []
    },
    "totalErrors": 1
  }
}
```

### Troubleshooting

#### Common Issues

**Authentication Failed**
- Verify WIZ_CLIENT_ID and WIZ_CLIENT_SECRET are correct
- Check if service account has necessary permissions
- Ensure WIZ_AUDIENCE is set to "beyond-api"

**No Data Imported**
- Check Wiz filters in sync request
- Verify Wiz account has data in specified cloud platforms
- Review API rate limits and quotas

**Partial Import Failures**
- Check error messages in sync response
- Verify asset relationships and dependencies
- Review data mapping configurations

#### Debug Mode

Enable detailed logging for troubleshooting:
```bash
# Set debug environment variable
DEBUG=wiz:* npm run dev

# View detailed sync logs
curl -X POST "http://localhost:5000/api/integrations/wiz/sync" \
  -H "Content-Type: application/json" \
  -d '{"debug": true}'
```

### Code Quality
- ESLint configuration for code standards
- Prettier for consistent formatting
- Type safety with strict TypeScript configuration
- Security scanning with automated tools

## License

This project is licensed under the MIT License. See LICENSE file for details.

## Support

For technical support, feature requests, or bug reports, please contact:
- Technical Support: support@ai-spm.com
- Documentation: docs@ai-spm.com
- Security Issues: security@ai-spm.com

---

Built with ❤️ for enterprise AI security
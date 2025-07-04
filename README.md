# AI Security Posture Management (AI-SPM) Platform

A comprehensive enterprise-grade security solution designed to manage and monitor AI/ML assets throughout their lifecycle. This platform provides comprehensive security governance for AI systems from development to production deployment, featuring advanced authentication, real-time security monitoring, AI/ML specific security controls, automated privacy governance, sophisticated adversarial attack detection, automated compliance workflows, and enterprise-grade data quality monitoring with anomaly detection.

## Key Features

### Advanced Authentication & Authorization
- **Multi-Factor Authentication**: OAuth 2.0/OpenID Connect, SAML, and FIDO2/WebAuthn support
- **Enterprise SSO Integration**: Seamless integration with enterprise identity providers
- **Hardware Security Keys**: FIDO2/WebAuthn for passwordless authentication
- **API Key Management**: Secure service-to-service authentication with scoped permissions
- **JWT Token Validation**: Service mesh integrated token validation with automatic refresh

### Enhanced Security Monitoring
- **Real-time Security Event Correlation**: Advanced pattern detection and behavioral analytics
- **Automated Incident Response**: Configurable workflows for threat remediation
- **SIEM Integration**: Native connectivity to Splunk, IBM QRadar, and other security platforms
- **Threat Intelligence Integration**: Automated IOC matching and threat hunting
- **Behavioral Analytics**: Machine learning-based anomaly detection for user and system behavior

### Advanced AI/ML Security Features
- **Model Versioning & Lineage**: Complete tracking of ML model lifecycle and dependencies
- **Automated Bias Detection**: Comprehensive fairness analysis with demographic parity and equalized odds
- **Federated Learning Security**: Monitoring and validation for distributed ML training
- **ML Pipeline Security Scanning**: Automated vulnerability assessment of ML workflows
- **AI Explainability Tools**: LIME, SHAP integration for model interpretability and compliance

### Real-Time Data Quality Monitoring
- **Comprehensive Quality Assessment**: Automated monitoring of completeness, accuracy, consistency, validity, uniqueness, and freshness
- **Data Drift Detection**: Statistical analysis using Kolmogorov-Smirnov, Chi-square, and Wasserstein distance tests
- **Advanced Anomaly Detection**: Ensemble methods combining Isolation Forest, LOF, DBSCAN, and statistical outlier detection
- **Real-Time Alerting**: Configurable thresholds with multi-channel notifications for critical data integrity issues
- **Automated Quality Scoring**: Weighted quality metrics with trend analysis and predictive insights

### Advanced Adversarial Attack Detection
- **Data Poisoning Protection**: Real-time detection of malicious training data with statistical analysis and gradient monitoring
- **Model Evasion Defense**: Automated detection of FGSM, PGD, C&W, and DeepFool attacks with instant input blocking
- **Privacy Attack Prevention**: Membership and attribute inference attack detection with differential privacy integration
- **Automated Response System**: Real-time threat blocking, asset quarantine, and multi-channel alerting

### Automated Compliance Assessment
- **Framework Support**: NIST AI RMF, EU AI Act, and GDPR compliance with automated evidence collection
- **Multi-Format Reporting**: Professional PDF, Excel, HTML, and JSON compliance reports
- **Gap Analysis**: Automated compliance gap identification with remediation recommendations
- **Evidence Validation**: Automated integrity checking and audit trail maintenance

### Data Privacy & Governance
- **Data Lineage Tracking**: Complete visibility into AI workflow data dependencies
- **Automated PII Detection**: Advanced classification with confidence scoring
- **Data Retention Policy Enforcement**: Automated lifecycle management with compliance tracking
- **GDPR/CCPA Compliance Automation**: Built-in privacy request handling and consent management
- **Differential Privacy Implementation**: Privacy-preserving analytics and model training

### Enterprise Architecture
- **Service Mesh Security**: Istio-based zero-trust architecture with automatic mTLS
- **Microservices Integration**: Specialized Python services for AI security tasks
- **Cloud-Native Deployment**: Kubernetes-ready with comprehensive observability
- **High Availability**: Multi-region deployment with automated failover

## ✅ **Platform Status: Fully Operational**

The AI Security Posture Management platform is currently **LIVE** and fully operational with all security and monitoring systems active:

### 🚀 **Core Systems Status**
- ✅ **Data Poisoning Detection** - Signatures initialized and monitoring active
- ✅ **Model Evasion Detection** - Real-time protection against adversarial attacks  
- ✅ **Membership Inference Detection** - Privacy protection systems operational
- ✅ **Attribute Inference Detection** - Sensitive data safeguards active
- ✅ **Adversarial Detection Manager** - Centralized threat coordination running
- ✅ **Data Quality Monitor** - Real-time quality assessment with default thresholds
- ✅ **Data Drift Detector** - Statistical distribution monitoring active
- ✅ **Anomaly Detector** - Ensemble detection methods operational
- ✅ **Data Quality Manager** - Orchestrated monitoring workflows running
- ✅ **GDPR Compliance Engine** - Automated privacy policy management active

### 🔧 **API Endpoints Available**
- **12 Data Quality Monitoring APIs** - Quality assessment, drift detection, anomaly analysis
- **8 Adversarial Detection APIs** - Threat detection and response management
- **10+ Compliance Assessment APIs** - Automated evidence collection and reporting
- **Complete REST API Suite** - Full platform management and monitoring capabilities

### 📊 **Monitoring & Alerting Active**
- **Real-time Quality Metrics** - Completeness, accuracy, consistency, validity, uniqueness, freshness
- **Multi-channel Notifications** - Slack, email, PagerDuty, SMS, webhook integrations
- **Configurable Thresholds** - Quality score, drift detection, anomaly rate monitoring
- **Automated Response System** - Threat blocking, asset quarantine, escalation policies

## Hybrid Microservices Architecture with Service Mesh

### Architecture Overview
The platform implements a modern hybrid microservices architecture with **Istio service mesh** that optimizes for both performance, security, and observability:

- **Node.js API Gateway**: Handles web services, authentication, and data management
- **Python Microservices**: Specialized services for AI/ML security tasks
- **React Frontend**: Modern, responsive user interface
- **PostgreSQL Database**: Centralized data storage with ORM integration
- **Istio Service Mesh**: Provides mTLS, traffic management, and observability

### Service Mesh Security Features
- **Automatic mTLS**: All inter-service communication is encrypted and authenticated
- **Zero Trust Security**: Services communicate only through verified certificates
- **Authorization Policies**: Fine-grained access control between services
- **Traffic Encryption**: End-to-end encryption for all service communications
- **Certificate Management**: Automatic certificate rotation and management

### Technology Stack

#### Frontend Layer
- **React 18** - Modern component-based UI framework
- **TypeScript** - Type-safe development with enhanced developer experience
- **Tailwind CSS** - Utility-first styling with responsive design
- **Shadcn/UI** - Production-ready component library
- **TanStack Query** - Powerful data synchronization and caching
- **React Hook Form** - Performant forms with validation
- **Recharts** - Interactive data visualization

#### Node.js API Gateway & Web Services
- **Node.js 18+** - High-performance JavaScript runtime
- **Express.js** - Fast, unopinionated web framework
- **TypeScript** - End-to-end type safety
- **Passport.js** - Comprehensive authentication strategies
- **Drizzle ORM** - Type-safe database operations
- **Zod** - Runtime type validation and parsing

#### Python Microservices
- **FastAPI** - High-performance async web framework
- **Python 3.9+** - AI/ML ecosystem compatibility
- **Pydantic** - Data validation and settings management
- **Uvicorn** - ASGI server for production deployment
- **Httpx** - Modern HTTP client for service communication

#### Data Layer
- **PostgreSQL 13+** - Enterprise-grade relational database
- **Connection pooling** - Optimized database connections
- **Database migrations** - Version-controlled schema management

#### Service Mesh Layer (Istio)
- **Istio 1.20+** - Production-ready service mesh
- **Envoy Proxy** - High-performance L7 proxy for all services
- **Automatic mTLS** - Zero-configuration mutual TLS encryption
- **Traffic Management** - Advanced routing, load balancing, and fault injection
- **Observability** - Distributed tracing, metrics, and access logs
- **Security Policies** - Authorization and authentication policies

### Microservices Architecture

#### 🤖 AI Scanner Service (Port 8001) - **OPERATIONAL**
- **Purpose**: AI/ML model security analysis and bias detection
- **Technology**: FastAPI, Python 3.9+
- **Capabilities**:
  - Model vulnerability scanning
  - Bias detection and fairness analysis
  - Security risk assessment
  - Model performance monitoring

#### 🔍 Data Integrity Service (Port 8002) - **OPERATIONAL**
- **Purpose**: Advanced data quality monitoring and anomaly detection
- **Technology**: FastAPI, Python 3.9+
- **Capabilities**:
  - Data quality validation
  - Anomaly detection algorithms
  - Data drift monitoring
  - Integrity reporting

#### 🔗 Wiz Integration Service (Port 8003) - **OPERATIONAL**
- **Purpose**: External security platform integration
- **Technology**: FastAPI, Python 3.9+, Httpx
- **Capabilities**:
  - Wiz API data transformation
  - Security alert processing
  - Cloud security posture integration
  - Real-time data synchronization

#### 📋 Compliance Engine (Port 8004) - **OPERATIONAL**
- **Purpose**: Automated compliance assessment and policy evaluation
- **Technology**: FastAPI, Python 3.9+
- **Capabilities**:
  - Multi-framework compliance checking
  - Policy rule evaluation
  - Automated assessment workflows
  - Compliance reporting

## Project Structure

```
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   │   ├── charts/     # Data visualization components
│   │   │   ├── dashboard/  # Dashboard-specific components
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
├── server/                 # Node.js API Gateway
│   ├── auth.ts            # Authentication middleware
│   ├── db.ts              # Database connection
│   ├── routes.ts          # API route definitions
│   ├── storage.ts         # Data access layer
│   ├── gateway.ts         # Microservices gateway
│   ├── microservices-gateway.ts # Service discovery
│   ├── index.ts           # Server entry point
│   ├── vite.ts            # Development server setup
│   ├── monitoring/        # Comprehensive monitoring system
│   │   ├── logger.ts      # Structured logging with Winston
│   │   ├── metrics-collector.ts # Prometheus metrics collection
│   │   ├── health-checker.ts    # Component health monitoring
│   │   └── notification-manager.ts # Multi-channel alerting
│   ├── routes/
│   │   ├── monitoring-routes.ts # Monitoring API endpoints
│   │   └── threat-config-routes.ts # Threat configuration APIs
│   └── config/            # Runtime configuration
│       ├── threat-detection-config.json # AI threat rules
│       └── compliance-policies.json     # Compliance policies
├── microservices/         # Python Microservices
│   ├── ai-scanner/        # AI security analysis service
│   │   ├── main.py        # FastAPI application
│   │   └── requirements.txt
│   ├── data-integrity/    # Data quality monitoring service
│   │   ├── main.py        # FastAPI application
│   │   └── requirements.txt
│   ├── wiz-integration/   # External integration service
│   │   ├── main.py        # FastAPI application
│   │   └── requirements.txt
│   └── compliance-engine/ # Compliance assessment service
│       ├── main.py        # FastAPI application
│       └── requirements.txt
├── shared/                # Shared code between services
│   └── schema.ts          # Database schema and validation
├── ARCHITECTURE.md        # Detailed system architecture
├── ARCHITECTURE_DIAGRAM.md # Visual architecture diagram
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

### Legacy Integration Endpoints (Redirected to Microservices)
```
GET  /api/integrations/wiz/status              # Check Wiz integration status
POST /api/integrations/wiz/sync-assets         # Redirects to microservice
POST /api/integrations/wiz/sync-vulnerabilities # Redirects to microservice
```

### Microservices API Endpoints

#### AI Scanner Service (Port 8001)
```
POST /scan/model           # Analyze AI model for security vulnerabilities
POST /scan/bias            # Detect bias in AI model predictions
GET  /scan/status/:id      # Get scan status and results
GET  /health               # Service health check
```

#### Data Integrity Service (Port 8002)
```
POST /check/quality        # Validate data quality
POST /check/anomalies      # Detect data anomalies
POST /check/drift          # Monitor data drift
GET  /health               # Service health check
```

#### Wiz Integration Service (Port 8003)
```
POST /integrate            # Process Wiz platform data
POST /transform/alerts     # Transform security alerts
POST /sync/assets          # Synchronize asset data
GET  /health               # Service health check
```

#### Compliance Engine (Port 8004)
```
POST /assess/framework     # Assess compliance against framework
POST /evaluate/policy      # Evaluate policy compliance
GET  /frameworks           # List available compliance frameworks
GET  /health               # Service health check
```

## Installation & Setup

### Prerequisites

#### For Local/Docker Development
- **Node.js 18+** - For API Gateway and frontend
- **Python 3.9+** - For microservices
- **PostgreSQL 13+** - Database server
- **npm or yarn** - Package manager
- **Docker 20.10+** - Container runtime
- **Docker Compose 2.0+** - Container orchestration

#### For Service Mesh Deployment
- **Kubernetes 1.24+** - Container orchestration platform
- **Istio 1.20+** - Service mesh platform
- **kubectl** - Kubernetes command-line tool
- **istioctl** - Istio command-line tool
- **Helm 3.0+** - Package manager for Kubernetes (optional)

### Environment Configuration
Create a `.env` file in the project root:
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

# Microservices Configuration
AI_SCANNER_URL=http://localhost:8001
DATA_INTEGRITY_URL=http://localhost:8002
WIZ_INTEGRATION_URL=http://localhost:8003
COMPLIANCE_ENGINE_URL=http://localhost:8004

# Wiz Integration (Optional)
WIZ_CLIENT_ID=your_wiz_client_id
WIZ_CLIENT_SECRET=your_wiz_client_secret
WIZ_AUDIENCE=beyond-api
```

### Installation Steps

#### 1. Clone and Install Node.js Dependencies
```bash
git clone <repository-url>
cd ai-spm-platform
npm install
```

#### 2. Database Setup
```bash
# Create PostgreSQL database
createdb ai_spm

# Push database schema
npm run db:push
```

#### 3. Set Up Python Microservices
Each microservice requires Python dependencies:

```bash
# AI Scanner Service
cd microservices/ai-scanner
pip install -r requirements.txt

# Data Integrity Service
cd ../data-integrity
pip install -r requirements.txt

# Wiz Integration Service
cd ../wiz-integration
pip install -r requirements.txt

# Compliance Engine
cd ../compliance-engine
pip install -r requirements.txt
cd ../..
```

#### 4. Start the Platform

**Option A: Start All Services (Recommended for Development)**
```bash
# Terminal 1: Start main application (API Gateway + Frontend)
npm run dev

# Terminal 2: Start AI Scanner microservice
cd microservices/ai-scanner && python main.py

# Terminal 3: Start Data Integrity microservice
cd microservices/data-integrity && python main.py

# Terminal 4: Start Wiz Integration microservice
cd microservices/wiz-integration && python main.py

# Terminal 5: Start Compliance Engine microservice
cd microservices/compliance-engine && python main.py
```

**Option B: Start Main Application Only**
```bash
npm run dev
```

The main application will be available at `http://localhost:5000`

#### 5. Verify Installation
- **Frontend**: Navigate to `http://localhost:5000`
- **API Gateway**: Check `http://localhost:5000/api/health`
- **Microservices Health**:
  - AI Scanner: `http://localhost:8001/health`
  - Data Integrity: `http://localhost:8002/health`
  - Wiz Integration: `http://localhost:8003/health`
  - Compliance Engine: `http://localhost:8004/health`

### Production Deployment

#### Option 1: Service Mesh Deployment (Recommended)
Deploy with Istio service mesh for enterprise security and observability:

```bash
# Install prerequisites
curl -L https://istio.io/downloadIstio | sh -
export PATH=$PWD/istio-1.20.0/bin:$PATH

# Deploy with service mesh
chmod +x deploy/service-mesh-deployment.sh
./deploy/service-mesh-deployment.sh deploy
```

**Service Mesh Features:**
- **Automatic mTLS** between all services
- **Authorization policies** for fine-grained access control  
- **Distributed tracing** with Jaeger
- **Metrics collection** with Prometheus
- **Traffic management** with intelligent routing

#### Option 2: Docker Compose Deployment
Deploy with Docker Compose for development/testing:

```bash
# Build and deploy all services
docker-compose up --build -d

# Or deploy only specific services
docker-compose up --build database api-gateway ai-scanner
```

#### Option 3: AWS ECS Deployment
Deploy using CloudFormation template:

```bash
# Build and push container images
aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin

# Deploy infrastructure
aws cloudformation deploy \
  --template-file cloudformation.yaml \
  --stack-name ai-spm-production \
  --capabilities CAPABILITY_IAM CAPABILITY_NAMED_IAM \
  --parameter-overrides EnableMicroservices=true
```

#### Option 4: API Gateway Only
Deploy just the Node.js API Gateway without microservices:
```bash
npm run build
npm start
```

## Architecture Benefits

### 🎯 **Technology Optimization**
- **Node.js**: Optimized for high-throughput web services and real-time data
- **Python**: Leverages rich AI/ML ecosystem for specialized security tasks
- **React**: Modern, responsive user interface with excellent developer experience
- **Istio Service Mesh**: Production-grade traffic management and security

### 🚀 **Scalability & Performance** 
- **Independent Scaling**: Scale web services and AI services based on different demand patterns
- **Resource Optimization**: Allocate resources efficiently based on service requirements
- **Load Distribution**: Distribute processing across multiple specialized services
- **Intelligent Routing**: Istio provides advanced load balancing and traffic splitting

### 🔧 **Development & Maintenance**
- **Team Specialization**: Web developers work on Node.js, AI/ML experts on Python services
- **Independent Deployment**: Deploy and update services independently
- **Clear Boundaries**: Well-defined service responsibilities and interfaces
- **Zero-Downtime Deployments**: Istio enables canary deployments and traffic shifting

### 🛡️ **Enterprise Security**
- **Service Isolation**: Security issues in one service don't affect others
- **Centralized Authentication**: Single point of authentication through API Gateway
- **Audit Trail**: Comprehensive logging across all services
- **Automatic mTLS**: All inter-service communication is encrypted and authenticated
- **Zero Trust Architecture**: Services must prove identity for every request
- **Policy Enforcement**: Fine-grained authorization policies between services

### 🔄 **Integration Flexibility**
- **API-First Design**: RESTful APIs for easy integration with existing systems  
- **Protocol Standardization**: Consistent HTTP/JSON communication
- **Service Discovery**: Automatic service registration and discovery
- **Circuit Breaking**: Automatic failure isolation and recovery

### 📊 **Observability & Monitoring**
- **Distributed Tracing**: End-to-end request tracing across all services
- **Metrics Collection**: Comprehensive performance and business metrics
- **Access Logging**: Detailed logs of all service communications
- **Real-time Dashboards**: Grafana, Kiali, and Jaeger integration

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

### 🚨 **Advanced Adversarial Attack Detection**
Real-time protection against sophisticated AI/ML security threats with automated response capabilities:

#### **Data Poisoning Detection Engine**
- **Statistical Analysis**: Z-score and IQR outlier detection for poisoned training samples
- **Distribution Monitoring**: Temporal shift detection comparing training vs validation data distributions
- **Correlation Analysis**: Feature correlation patterns to identify suspicious data relationships
- **Gradient Anomaly Detection**: Training gradient analysis to detect manipulation during model updates
- **Ensemble Validation**: Cross-model consistency checks to identify dataset integrity issues

#### **Model Evasion Attack Protection**
- **Real-time Adversarial Detection**: Automated detection of FGSM, PGD, C&W, DeepFool attacks
- **Input Preprocessing Defense**: Anomaly detection in model inputs before inference
- **Confidence Analysis**: Prediction confidence scoring with ensemble disagreement detection
- **Automated Input Blocking**: Instant blocking of malicious inputs with configurable thresholds
- **Gradient Analysis**: Attack signature detection through gradient magnitude monitoring

#### **Membership Inference Privacy Protection**
- **Privacy Attack Detection**: Statistical analysis of confidence patterns indicating training data membership
- **Shadow Model Defense**: Comparison techniques to detect membership inference attempts
- **Overfitting Indicators**: Detection of model behavior suggesting privacy vulnerabilities
- **Information Leakage Quantification**: Mutual information analysis for privacy risk assessment
- **Differential Privacy Integration**: Configurable noise injection for privacy preservation

#### **Attribute Inference Safeguards**
- **Sensitive Attribute Protection**: Detection of attempts to infer protected characteristics (age, gender, income)
- **Correlation Monitoring**: Analysis of prediction-attribute correlations indicating privacy leakage
- **Auxiliary Model Detection**: Identification of attacks using external models for attribute inference
- **Feature Importance Analysis**: Monitoring for sensitive attribute influence in model decisions
- **Privacy Leakage Scoring**: Quantitative assessment of attribute inference vulnerability

#### **Automated Response System**
- **Real-time Threat Blocking**: Immediate blocking of malicious inputs with sub-second response times
- **Asset Quarantine**: Automated isolation of compromised models and datasets
- **Multi-channel Alerting**: Instant notifications via Slack, email, PagerDuty, SMS, and webhooks
- **Escalation Policies**: Configurable incident response workflows with severity-based escalation
- **Audit Trail**: Comprehensive logging of all detection events and response actions for compliance

### **API Endpoints for Adversarial Detection**

#### Data Poisoning Detection
```bash
POST /api/adversarial-detection/data-poisoning/analyze
{
  "datasetId": "dataset_123",
  "samples": [{ "id": "sample_1", "features": [1.2, 3.4, ...], "label": "normal" }],
  "modelPredictions": [{ "modelId": "model_1", "predictions": [...] }]
}
```

#### Model Evasion Detection
```bash
POST /api/adversarial-detection/model-evasion/analyze
{
  "inputSample": { "id": "input_1", "features": [1.2, 3.4, ...] },
  "predictions": [{ "modelId": "model_1", "prediction": "normal", "confidence": 0.95 }],
  "baselineInput": { "id": "baseline_1", "features": [1.0, 3.0, ...] }
}
```

#### Membership Inference Detection
```bash
POST /api/adversarial-detection/membership-inference/analyze
{
  "queryId": "query_123",
  "modelId": "model_1",
  "samples": [{ "id": "sample_1", "confidence": 0.95, "loss": 0.05 }],
  "shadowPredictions": [{ "modelId": "shadow_1", "membershipScore": 0.8 }]
}
```

#### Attribute Inference Detection
```bash
POST /api/adversarial-detection/attribute-inference/analyze
{
  "queryId": "query_123", 
  "modelId": "model_1",
  "samples": [{ "prediction": "positive", "knownAttributes": { "age": 30 } }],
  "targetAttributes": ["age", "gender", "income"]
}
```

#### Management & Statistics
```bash
GET /api/adversarial-detection/stats              # Detection statistics
GET /api/adversarial-detection/quarantine         # Quarantined assets
POST /api/adversarial-detection/quarantine/release # Release from quarantine
GET /api/adversarial-detection/incidents          # Active incidents
PUT /api/adversarial-detection/config             # Update response configuration
POST /api/adversarial-detection/test              # Test with sample data
```

### 📋 **NEW: Automated Compliance Assessment Workflows**
Comprehensive compliance management system with evidence collection and automated report generation for regulatory frameworks:

#### **Evidence Collection Engine**
- **Automated Evidence Gathering**: Systematic collection from configuration files, audit logs, scan results, and policy documents
- **Framework-Specific Mapping**: Evidence requirements mapped to NIST AI RMF, EU AI Act, and GDPR controls
- **Real-time Validation**: Integrity checks with hash verification and freshness validation
- **Scheduled Collection**: Configurable automatic evidence collection with retention policies
- **Multi-source Integration**: Collects from databases, configuration files, security scans, and external systems

#### **Compliance Report Generator**
- **Multi-Format Reports**: PDF, Excel, HTML, and JSON output formats with professional styling
- **Framework Templates**: Pre-configured templates for NIST AI RMF, EU AI Act, and GDPR compliance
- **Executive Summaries**: High-level compliance scores with critical findings and recommendations
- **Detailed Technical Reports**: Comprehensive evidence inventory with gap analysis
- **Automated Remediation Plans**: Priority-based recommendations with implementation timelines

#### **Compliance Assessment Features**
- **Gap Analysis**: Automated identification of missing evidence and non-compliant controls
- **Risk Scoring**: Quantitative compliance scores with risk level classification
- **Evidence Validation**: Automated verification of evidence integrity and completeness
- **Audit Trail**: Comprehensive logging of all compliance activities for regulatory requirements
- **Real-time Monitoring**: Continuous compliance status tracking with alerting

### **API Endpoints for Compliance Management**

#### Evidence Collection
```bash
POST /api/compliance/evidence/collect
{
  "framework": "nist_ai_rmf" | "eu_ai_act" | "gdpr",
  "dateRange": {
    "startDate": "2024-01-01T00:00:00Z",
    "endDate": "2024-12-31T23:59:59Z"
  }
}
```

#### Report Generation
```bash
POST /api/compliance/reports/generate
{
  "framework": "nist_ai_rmf" | "eu_ai_act" | "gdpr",
  "reportType": "executive_summary" | "detailed_technical" | "compliance_gap_analysis" | "evidence_inventory" | "risk_assessment" | "remediation_plan",
  "format": "pdf" | "excel" | "html" | "json",
  "includeEvidence": true,
  "includeRecommendations": true,
  "branding": {
    "companyName": "Your Company",
    "colors": {
      "primary": "#337ab7",
      "secondary": "#5bc0de"
    }
  }
}
```

#### Evidence Management
```bash
GET  /api/compliance/evidence/stats              # Evidence collection statistics
POST /api/compliance/evidence/schedule           # Schedule automatic collection
DELETE /api/compliance/evidence/schedule/:framework # Stop scheduled collection
POST /api/compliance/evidence/test               # Test evidence collection
```

#### Compliance Framework Management
```bash
GET /api/compliance/frameworks                   # Available frameworks and options
GET /api/compliance/reports/stats                # Report generation statistics
GET /api/compliance/reports/download/:reportId   # Download generated reports
```

#### **Supported Compliance Frameworks**

##### **NIST AI Risk Management Framework (AI RMF)**
- **AI-1.1**: AI governance structure and roles documentation
- **AI-2.1**: AI risk assessment and management processes  
- **AI-3.1**: AI system security testing and vulnerability assessment
- **AI-4.1**: AI system monitoring and incident response

##### **EU AI Act Compliance**
- **AIA-9.1**: Risk management system for high-risk AI applications
- **AIA-10.1**: Data governance and quality management processes
- **AIA-11.1**: Record-keeping and transparency requirements
- **AIA-12.1**: Accuracy, robustness and cybersecurity measures

##### **GDPR Data Protection Compliance**
- **GDPR-32**: Security of processing - technical and organisational measures
- **GDPR-30**: Records of processing activities
- **GDPR-35**: Data protection impact assessments
- **GDPR-33**: Personal data breach notification procedures

#### **Evidence Types Collected**
- **Configuration Evidence**: System configurations, threat detection settings, compliance policies
- **Audit Logs**: User activities, system events, security incidents with 7-year retention
- **Scan Results**: Vulnerability assessments, security testing results, risk evaluations
- **Policy Documents**: Compliance policies, procedures, governance frameworks
- **Security Alerts**: Incident reports, threat detections, response actions
- **Training Records**: Security and compliance training completion records
- **Risk Assessments**: AI asset risk evaluations, impact analyses, mitigation strategies
- **Data Flow Diagrams**: System architecture, data processing flows, privacy impact assessments

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

### 📊 **Real-Time Data Quality Monitoring API**

Comprehensive data quality monitoring with advanced anomaly detection and drift analysis for AI/ML datasets:

#### **Data Quality Monitoring**
```bash
# Monitor dataset quality with comprehensive metrics
curl -X POST http://localhost:3000/api/data-quality/monitor \
  -H "Content-Type: application/json" \
  -d '{
    "assetId": 123,
    "datasetName": "training_data",
    "currentData": [...],
    "referenceData": [...],
    "environment": "training"
  }'
```

#### **Generate Quality Report**
```bash
# Generate comprehensive quality report
curl -X GET "http://localhost:3000/api/data-quality/report?assetId=123&timeRange=24h"
```

#### **Anomaly Detection**
```bash
# Detect anomalies in dataset using ensemble methods
curl -X POST http://localhost:3000/api/data-quality/anomalies/detect \
  -H "Content-Type: application/json" \
  -d '{
    "assetId": 123,
    "datasetName": "inference_data",
    "data": [...],
    "environment": "inference"
  }'
```

#### **Data Drift Detection**
```bash
# Detect data drift between datasets
curl -X POST http://localhost:3000/api/data-quality/drift/detect \
  -H "Content-Type: application/json" \
  -d '{
    "assetId": 123,
    "referenceData": [...],
    "currentData": [...],
    "environment": "production"
  }'
```

#### **Quality Baselines**
```bash
# Create quality baseline for reference
curl -X POST http://localhost:3000/api/data-quality/baselines \
  -H "Content-Type: application/json" \
  -d '{
    "assetId": 123,
    "datasetName": "training_baseline",
    "baselineMetrics": {
      "completeness": 0.95,
      "accuracy": 0.92,
      "consistency": 0.88
    },
    "environment": "training"
  }'
```

#### **Validation Rules**
```bash
# Configure custom validation rules
curl -X POST http://localhost:3000/api/data-quality/validation-rules \
  -H "Content-Type: application/json" \
  -d '{
    "assetId": 123,
    "ruleName": "age_range_validation",
    "ruleType": "range",
    "field": "age",
    "parameters": {"min": 18, "max": 100}
  }'
```

#### **Monitoring Configuration**
```bash
# Update monitoring configuration
curl -X PUT http://localhost:3000/api/data-quality/config \
  -H "Content-Type: application/json" \
  -d '{
    "enableRealTimeMonitoring": true,
    "monitoringInterval": 15,
    "enableDriftDetection": true,
    "enableAnomalyDetection": true,
    "alertThresholds": {
      "qualityScoreThreshold": 0.8,
      "driftThreshold": 0.3,
      "anomalyRateThreshold": 0.05
    }
  }'
```

#### **Quality Metrics**
```bash
# Get quality metrics for asset
curl -X GET "http://localhost:3000/api/data-quality/metrics?assetId=123&timeRange=7d"
```

#### **Start/Stop Monitoring**
```bash
# Start automated monitoring
curl -X POST http://localhost:3000/api/data-quality/monitoring/start

# Stop automated monitoring
curl -X POST http://localhost:3000/api/data-quality/monitoring/stop

# Get monitoring status
curl -X GET http://localhost:3000/api/data-quality/monitoring/status
```

#### **Data Quality Response Examples**

**Quality Report Response:**
```json
{
  "assetId": 123,
  "datasetName": "training_data",
  "generatedAt": "2024-01-15T10:30:00Z",
  "qualityOverview": {
    "overallScore": 0.85,
    "status": "good",
    "totalRecords": 10000,
    "validRecords": 8500,
    "qualityTrend": "stable"
  },
  "qualityMetrics": {
    "completeness": 0.92,
    "accuracy": 0.88,
    "consistency": 0.85,
    "validity": 0.90,
    "uniqueness": 0.95,
    "freshness": 0.80
  },
  "driftAnalysis": {
    "overallDriftScore": 0.15,
    "driftStatus": "stable",
    "driftedFeatures": 2,
    "totalFeatures": 15,
    "recommendations": [
      "Monitor feature 'income' for continued drift",
      "Consider retraining if drift persists"
    ]
  },
  "anomalyAnalysis": {
    "totalAnomalies": 45,
    "anomalyRate": 0.0045,
    "severityDistribution": {
      "low": 25,
      "medium": 15,
      "high": 4,
      "critical": 1
    },
    "dominantAnomalyTypes": ["statistical_outlier", "pattern_anomaly"]
  }
}
```

**Anomaly Detection Response:**
```json
{
  "datasetName": "inference_data",
  "assetId": 123,
  "totalRecords": 1000,
  "anomalousRecords": 12,
  "anomalyPercentage": 1.2,
  "detectionResults": [
    {
      "recordId": "record_789",
      "anomalyScore": 0.85,
      "confidence": 0.92,
      "anomalyType": "statistical_outlier",
      "detectionMethod": "isolation_forest",
      "affectedFeatures": ["age", "income"],
      "severity": "high"
    }
  ],
  "alerts": [
    {
      "alertType": "high_anomaly_rate",
      "severity": "medium",
      "title": "Elevated Anomaly Rate Detected",
      "description": "Anomaly rate of 1.2% exceeds threshold of 1.0%"
    }
  ]
}
```

### Code Quality
- ESLint configuration for code standards
- Prettier for consistent formatting
- Type safety with strict TypeScript configuration
- Security scanning with automated tools

## 🎯 **Latest Implementation Achievements**

### ✅ **July 2025 Major Release - Enterprise Data Quality Monitoring**
Successfully deployed comprehensive enterprise-grade data quality monitoring platform with:

**Real-Time Data Quality Assessment**
- Automated monitoring of 6 core quality metrics (completeness, accuracy, consistency, validity, uniqueness, freshness)
- Configurable quality thresholds with weighted scoring algorithms
- Real-time quality trend analysis and predictive insights

**Advanced Data Drift Detection**
- Statistical analysis using Kolmogorov-Smirnov, Chi-square, and Wasserstein distance tests
- Distribution shift monitoring for numerical and categorical features
- Temporal pattern analysis with configurable sensitivity thresholds

**Ensemble Anomaly Detection**
- Sophisticated anomaly detection combining Isolation Forest, LOF, DBSCAN, and statistical outlier methods
- Multi-layer anomaly scoring with confidence estimation
- Pattern-based anomaly detection for temporal and sequential data

**Production-Ready Integration**
- Complete REST API with 12 endpoints for quality monitoring, anomaly detection, and drift analysis
- Real-time alerting system with multi-channel notifications (Slack, email, PagerDuty, SMS, webhooks)
- Automated response system with threat blocking, asset quarantine, and escalation policies
- Comprehensive audit trails and compliance documentation

**Enterprise Architecture**
- Extended database schema with 6 new tables for quality metrics, drift detection, and anomaly tracking
- Orchestrated monitoring architecture with Data Quality Manager coordinating all components
- Integration with existing adversarial detection and compliance assessment systems
- Production-grade logging, monitoring, and health check capabilities

## License

This project is licensed under the MIT License. See LICENSE file for details.

## Support

For technical support, feature requests, or bug reports, please contact:
- Technical Support: support@ai-spm.com
- Documentation: docs@ai-spm.com
- Security Issues: security@ai-spm.com

---

Built with ❤️ for enterprise AI security
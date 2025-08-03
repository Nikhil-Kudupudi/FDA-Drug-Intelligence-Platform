# FDA Drug Intelligence Platform 
> **Comprehensive architectures  for creating professional system diagrams using any diagramming tool (Lucidchart, Draw.io, Mermaid, etc.)**

## 🏗️ Master System Architecture Prompt

### **Complete End-to-End Architecture**

**Use this prompt for creating the main system architecture diagram:**

```
Create a comprehensive system architecture diagram for "FDA Drug Intelligence Platform" showing:

**DATA SOURCES LAYER:**
- FDA OpenFDA API (external data source)
- Real-time data feeds
- Historical data archives
- Supplementary pharmaceutical databases

**DATA INGESTION LAYER:**
- Python ETL Scripts (data extraction)
- Prefect Workflow Orchestration (scheduling & monitoring)
- Data Validation Gateway (quality checks)
- Error Handling & Retry Logic

**DATA STORAGE LAYER:**
- Supabase PostgreSQL (primary database)
- Redis Cache (performance optimization)
- File Storage (data backups & archives)
- Real-time Database Subscriptions

**DATA PROCESSING LAYER:**
- Python Data Processing (pandas, numpy)
- R Statistical Analysis (advanced statistics)
- Feature Engineering Pipeline
- Data Quality Monitoring

**API LAYER:**
- FastAPI Application Server
- Auto-generated REST APIs (Supabase)
- Authentication & Authorization
- Rate Limiting & Security
- API Gateway & Load Balancing

**ANALYTICS LAYER:**
- Business Intelligence Engine
- Statistical Analysis Modules
- KPI Calculation Engine
- Real-time Analytics Processing
- Market Intelligence Algorithms

**MACHINE LEARNING LAYER:**
- Feature Store & Engineering
- ML Model Training Pipeline
- MLflow Experiment Tracking
- Model Registry & Versioning
- A/B Testing Framework
- Model Serving APIs

**VISUALIZATION LAYER:**
- Power BI Dashboards (executive reporting)
- Streamlit Applications (interactive data apps)
- Jupyter Notebooks (exploratory analysis)
- Real-time Dashboard Updates
- Mobile-responsive Design

**DEPLOYMENT LAYER:**
- Railway/Render (backend hosting)
- Vercel (frontend hosting)
- GitHub Actions (CI/CD pipeline)
- Docker Containerization
- Environment Management

**MONITORING LAYER:**
- Application Performance Monitoring
- Database Performance Tracking
- API Health Checks
- Data Pipeline Monitoring
- ML Model Performance Tracking

**DATA FLOW CONNECTIONS:**
Show arrows indicating data flow from FDA API → ETL → Database → APIs → Dashboards → ML Models → Predictions

**TECHNOLOGY LABELS:**
Label each component with specific technologies (Python, Prefect, Supabase, FastAPI, Power BI, etc.)

**COLOR CODING:**
- Blue: Data ingestion and storage
- Green: Processing and analytics
- Orange: APIs and services
- Purple: Machine learning
- Red: Visualization and user interface
- Gray: Infrastructure and deployment

**INTEGRATION POINTS:**
Highlight key integration points between systems and show bidirectional data flows where applicable.
```

---

## 🔧 Data Engineering Architecture Prompt

### **Data Pipeline & ETL Architecture**

**Use this prompt for detailed data engineering diagrams:**

```
Create a detailed data engineering architecture diagram showing:

**DATA SOURCES:**
- FDA OpenFDA API (primary source)
- Rate limiting considerations (240 requests/minute)
- API authentication and access patterns
- Data availability and update schedules

**EXTRACTION LAYER:**
- Python Data Extractors
- API request handling and pagination
- Error handling and retry mechanisms
- Data source monitoring and health checks

**TRANSFORMATION LAYER:**
- Python Data Processing (pandas operations)
- Data Cleaning and Validation Rules
- Schema Mapping and Standardization
- Data Quality Checks and Reporting
- Business Rule Application

**LOADING LAYER:**
- Supabase PostgreSQL Target
- Batch and Real-time Loading
- Upsert Operations (handle duplicates)
- Data Archiving and Retention
- Performance Optimization

**ORCHESTRATION:**
- Prefect Workflow Management
- Task Dependencies and Scheduling
- Error Handling and Notifications
- Pipeline Monitoring and Alerting
- Resource Management and Scaling

**DATA FLOW STAGES:**
1. API Request → 2. Data Extraction → 3. Data Validation → 
4. Data Transformation → 5. Quality Checks → 6. Database Loading → 
7. Cache Updates → 8. Monitoring & Alerts

**PERFORMANCE OPTIMIZATION:**
- Redis Caching Layer
- Database Indexing Strategy
- Query Optimization
- Connection Pooling
- Resource Monitoring

**ERROR HANDLING:**
- Data Quality Validation Gates
- Pipeline Failure Recovery
- Dead Letter Queues
- Notification Systems
- Manual Intervention Triggers

**MONITORING & OBSERVABILITY:**
- Pipeline Health Dashboards
- Data Quality Metrics
- Performance Monitoring
- Error Tracking and Alerting
- SLA Monitoring

Include timing annotations (daily runs, real-time processing) and show both batch and streaming data paths.
```

---

## 📊 Analytics & Business Intelligence Architecture Prompt

### **Analytics Layer Architecture**

**Use this prompt for analytics-focused diagrams:**

```
Create a comprehensive analytics architecture diagram showing:

**RAW DATA LAYER:**
- Supabase PostgreSQL (normalized drug approval data)
- Historical data tables (5+ years of FDA approvals)
- Reference data (companies, therapeutic areas)
- Metadata and data lineage tracking

**DATA TRANSFORMATION LAYER:**
- SQL Aggregation Queries
- Business Logic Implementation
- KPI Calculation Engine
- Statistical Analysis Modules
- Data Mart Creation

**ANALYTICS ENGINE:**
- Python Analytics (pandas, numpy, scipy)
- R Statistical Analysis (tidyverse, forecast)
- Business Intelligence Calculations
- Market Intelligence Algorithms
- Trend Analysis and Forecasting

**ANALYTICAL DATABASES:**
- Optimized Query Tables
- Materialized Views for Performance
- Analytical Indexes
- Data Warehouse Star Schema
- OLAP Cube Structures

**API LAYER:**
- FastAPI Analytics Endpoints
- Real-time Query Processing
- Caching Strategy (Redis)
- Response Optimization
- Authentication & Rate Limiting

**VISUALIZATION SERVICES:**
- Power BI Data Connections
- Streamlit Backend Services
- Chart.js Data Preparation
- Export Services (PDF, CSV)
- Real-time Update Mechanisms

**BUSINESS INTELLIGENCE OUTPUTS:**
- Executive Dashboards
- Operational Reports
- Market Intelligence Briefings
- Competitive Analysis Reports
- Trend Analysis Summaries

**USER INTERFACES:**
- Power BI Reports (executive level)
- Streamlit Applications (interactive exploration)
- Jupyter Notebooks (analytical workflows)
- Mobile-responsive Dashboards
- Automated Report Distribution

**ANALYTICS WORKFLOWS:**
1. Raw Data → 2. Business Rules → 3. Aggregations → 
4. Statistical Analysis → 5. Insight Generation → 6. Visualization → 
7. Distribution → 8. User Interaction

Show different analytical paths for different user personas (executives, analysts, researchers).
```

---

## 🤖 Machine Learning Architecture Prompt

### **ML Pipeline & Model Serving Architecture**

**Use this prompt for ML-focused diagrams:**

```
Create a detailed machine learning architecture diagram showing:

**DATA PREPARATION:**
- Feature Store (engineered features from FDA data)
- Data Preprocessing Pipeline
- Feature Engineering Automation
- Data Validation and Quality Checks
- Training/Testing Data Splits

**MODEL DEVELOPMENT:**
- Python ML Environment (scikit-learn, XGBoost)
- Jupyter Notebooks (model experimentation)
- Automated Hyperparameter Tuning
- Cross-validation and Model Selection
- Model Evaluation and Comparison

**EXPERIMENT TRACKING:**
- MLflow Tracking Server
- Experiment Logging and Management
- Model Metadata and Lineage
- Performance Metrics Storage
- Artifact Management (models, plots, data)

**MODEL REGISTRY:**
- MLflow Model Registry
- Model Versioning and Staging
- Model Approval Workflows
- Model Deployment Automation
- Rollback Capabilities

**MODEL SERVING:**
- FastAPI Prediction Endpoints
- Model Loading and Caching
- Real-time Inference Processing
- Batch Prediction Capabilities
- Response Formatting and Validation

**A/B TESTING FRAMEWORK:**
- Traffic Splitting Logic
- Experiment Configuration
- Statistical Significance Testing
- Performance Comparison
- Results Analysis and Reporting

**MODEL MONITORING:**
- Prediction Performance Tracking
- Data Drift Detection
- Model Drift Monitoring
- Real-time Alerting
- Automated Retraining Triggers

**PREDICTION WORKFLOWS:**
1. Input Data → 2. Feature Engineering → 3. Model Loading → 
4. Prediction Generation → 5. Confidence Scoring → 6. Response Formatting → 
7. Logging & Monitoring → 8. User Interface Display

**FEEDBACK LOOP:**
Model Performance → Monitoring → Retraining → Updated Models → Improved Predictions

**INTEGRATION POINTS:**
- Dashboard Integration (prediction displays)
- API Integration (real-time predictions)
- Database Integration (prediction storage)
- Analytics Integration (model performance metrics)

Include model lifecycle stages (development, staging, production, retirement) and show both real-time and batch prediction paths.
```

---

## 🎨 Dashboard & Frontend Architecture Prompt

### **User Interface & Visualization Architecture**

**Use this prompt for frontend and visualization diagrams:**

```
Create a comprehensive frontend and visualization architecture showing:

**USER ACCESS LAYER:**
- Web Browsers (desktop and mobile)
- Authentication Gateway
- User Role Management
- Session Management
- Security Controls

**FRONTEND APPLICATIONS:**
- Power BI Dashboards (executive reporting)
- Streamlit Applications (interactive data exploration)
- Jupyter Notebooks (analytical workflows)
- Custom Web Interfaces
- Mobile-responsive Design

**VISUALIZATION COMPONENTS:**
- Chart.js (standard business charts)
- D3.js (custom interactive visualizations)
- Plotly (scientific and statistical plots)
- Maps and Geographic Visualizations
- Real-time Data Displays

**DATA CONNECTION LAYER:**
- REST API Clients
- WebSocket Connections (real-time updates)
- Database Direct Connections (Power BI)
- File-based Data Sources
- Cached Data Access

**BACKEND SERVICES:**
- FastAPI Application Server
- Supabase Auto-generated APIs
- Authentication Services
- Caching Layer (Redis)
- Real-time Subscription Services

**DATA PROCESSING FOR UI:**
- Data Aggregation for Charts
- Real-time Data Streaming
- Export Processing (PDF, CSV)
- User Preference Management
- Dashboard Configuration

**USER INTERACTION FLOWS:**
1. User Login → 2. Dashboard Loading → 3. Data Filtering → 
4. Chart Interaction → 5. Drill-down Analysis → 6. Export Results → 
7. Save Preferences → 8. Share Insights

**RESPONSIVE DESIGN:**
- Desktop Layout (full feature set)
- Tablet Layout (optimized interactions)
- Mobile Layout (essential features)
- Progressive Web App Features
- Offline Capabilities

**REAL-TIME FEATURES:**
- Live Data Updates
- Push Notifications
- Collaborative Features
- Auto-refresh Mechanisms
- Real-time Alerts

**PERFORMANCE OPTIMIZATION:**
- Lazy Loading
- Data Virtualization
- Caching Strategies
- Bundle Optimization
- CDN Integration

Show user personas (executives, analysts, researchers) and their specific interface requirements and data access patterns.
```

---

## ☁️ Deployment & Infrastructure Architecture Prompt

### **Cloud Infrastructure & DevOps Architecture**

**Use this prompt for deployment and infrastructure diagrams:**

```
Create a comprehensive cloud deployment architecture showing:

**DEVELOPMENT ENVIRONMENT:**
- Local Development Setup
- Docker Compose Services
- Local Database (Supabase local)
- Development Tools Integration
- Hot Reload and Testing

**SOURCE CODE MANAGEMENT:**
- GitHub Repository
- Branch Strategy (main, develop, feature branches)
- Pull Request Workflows
- Code Review Process
- Release Management

**CI/CD PIPELINE:**
- GitHub Actions Workflows
- Automated Testing (unit, integration, e2e)
- Code Quality Checks (linting, security scanning)
- Build Process (Docker images, frontend bundles)
- Deployment Automation

**STAGING ENVIRONMENT:**
- Railway/Render Staging Deployment
- Supabase Staging Database
- Redis Staging Instance
- Integration Testing Environment
- Performance Testing Setup

**PRODUCTION ENVIRONMENT:**
- Railway/Render Production Hosting (APIs)
- Vercel Production Hosting (frontend)
- Supabase Production Database
- Redis Cloud Production Cache
- CDN and Load Balancing

**MONITORING & OBSERVABILITY:**
- Application Performance Monitoring
- Database Performance Tracking
- API Health Checks and Uptime Monitoring
- Error Tracking and Alerting
- Log Aggregation and Analysis

**SECURITY LAYER:**
- SSL/TLS Encryption
- API Authentication and Authorization
- Database Security (RLS, encryption)
- Network Security Groups
- Secrets Management

**BACKUP & DISASTER RECOVERY:**
- Automated Database Backups
- Point-in-time Recovery
- Cross-region Replication
- Disaster Recovery Procedures
- Business Continuity Planning

**SCALING STRATEGY:**
- Horizontal API Scaling
- Database Read Replicas
- CDN Edge Caching
- Auto-scaling Configuration
- Load Balancing

**DEPLOYMENT FLOW:**
1. Code Commit → 2. Automated Tests → 3. Security Scan → 
4. Build Artifacts → 5. Deploy to Staging → 6. Integration Tests → 
7. Manual Approval → 8. Production Deployment → 9. Health Checks → 
10. Monitoring & Alerts

**ENVIRONMENT PROMOTION:**
Development → Staging → Production (with proper gates and approvals)

Include network diagrams, security boundaries, and data flow between environments.
```

---

## 📊 Data Flow Architecture Prompt

### **End-to-End Data Flow Diagram**

**Use this prompt for data flow visualization:**

```
Create a comprehensive data flow diagram for the FDA Drug Intelligence Platform showing:

**EXTERNAL DATA SOURCES:**
- FDA OpenFDA API (primary source)
- Rate limiting and API constraints
- Data update schedules and patterns
- Data quality and reliability

**DATA INGESTION FLOW:**
FDA API → HTTP Requests → Rate Limiting → Data Extraction → 
Format Validation → Error Handling → Raw Data Storage

**ETL PROCESSING FLOW:**
Raw Data → Data Cleaning → Schema Validation → Business Rules → 
Data Transformation → Quality Checks → Enrichment → Standardization

**DATABASE FLOW:**
Processed Data → Database Insertion → Index Updates → 
Materialized View Refresh → Cache Invalidation → Real-time Notifications

**ANALYTICS FLOW:**
Database → SQL Queries → Business Logic → Statistical Analysis → 
KPI Calculations → Aggregations → Cache Storage → API Responses

**MACHINE LEARNING FLOW:**
Historical Data → Feature Engineering → Model Training → 
Experiment Tracking → Model Validation → Model Registry → 
Production Deployment → Real-time Predictions

**VISUALIZATION FLOW:**
APIs → Data Formatting → Chart Data Preparation → 
Dashboard Rendering → User Interactions → Export Generation

**REAL-TIME DATA FLOW:**
New FDA Data → Immediate Processing → Database Updates → 
Cache Refresh → WebSocket Notifications → Dashboard Updates → 
User Notifications

**USER INTERACTION FLOW:**
User Request → Authentication → API Gateway → Business Logic → 
Database Query → Result Processing → Response Caching → 
User Interface Update

**BATCH PROCESSING FLOW:**
Scheduled Jobs → Data Processing → Bulk Operations → 
Performance Optimization → Monitoring → Completion Notifications

**MONITORING FLOW:**
System Metrics → Performance Data → Health Checks → 
Alert Generation → Notification Delivery → Issue Resolution

**DATA LIFECYCLE:**
Data Ingestion → Processing → Storage → Analysis → Visualization → 
Archival → Retention → Deletion

**SECURITY FLOW:**
User Authentication → Authorization Checks → Data Access Controls → 
Audit Logging → Security Monitoring → Compliance Reporting

Show data volumes, processing times, and performance characteristics at each stage.
Include error handling paths and data quality validation points.
Use different arrow styles for real-time vs batch processing flows.
```

---

## 🔧 Technical Component Architecture Prompt

### **Detailed Technical Stack Diagram**

**Use this prompt for technical implementation details:**

```
Create a detailed technical component architecture showing:

**PROGRAMMING LANGUAGES:**
- Python 3.9+ (primary backend language)
- R 4.2+ (statistical analysis)
- SQL (database operations)
- JavaScript/TypeScript (frontend interfaces)
- Shell Scripts (automation and deployment)

**BACKEND FRAMEWORKS:**
- FastAPI (modern Python web framework)
- Prefect (workflow orchestration)
- SQLAlchemy (database ORM)
- Pydantic (data validation)
- Asyncio (asynchronous processing)

**DATABASE TECHNOLOGIES:**
- PostgreSQL (primary database - via Supabase)
- Redis (caching and session storage)
- Database Migrations (schema versioning)
- Connection Pooling
- Query Optimization

**DATA PROCESSING LIBRARIES:**
- pandas (data manipulation)
- numpy (numerical computing)
- scipy (statistical analysis)
- requests (HTTP client for APIs)
- Beautiful Soup (data parsing if needed)

**MACHINE LEARNING STACK:**
- scikit-learn (traditional ML algorithms)
- XGBoost (gradient boosting)
- MLflow (experiment tracking)
- TensorFlow/Keras (deep learning)
- Joblib (model serialization)

**ANALYTICS & VISUALIZATION:**
- matplotlib/seaborn (Python plotting)
- plotly (interactive visualizations)
- streamlit (web applications)
- jupyter (notebook analysis)
- R packages (ggplot2, dplyr, tidyverse)

**API & WEB TECHNOLOGIES:**
- REST API design patterns
- OpenAPI/Swagger documentation
- CORS handling
- Rate limiting implementation
- Authentication (JWT tokens)

**CLOUD SERVICES:**
- Supabase (database-as-a-service)
- Railway/Render (application hosting)
- Vercel (frontend hosting)
- Redis Cloud (managed caching)
- GitHub (source code management)

**DEVOPS TOOLS:**
- Docker (containerization)
- GitHub Actions (CI/CD)
- pytest (testing framework)
- Black (code formatting)
- Flake8 (code linting)

**MONITORING & LOGGING:**
- Application logging (Python logging)
- Performance monitoring
- Error tracking
- Health check endpoints
- Metrics collection

**INTEGRATION PATTERNS:**
- RESTful API consumption
- Database connection management
- Caching strategies
- Background job processing
- Real-time data synchronization

**COMPONENT INTERACTIONS:**
Show how each technology component interacts with others, including:
- Data flow between components
- API calls and responses
- Database read/write operations
- Caching mechanisms
- Authentication flows

**PERFORMANCE CONSIDERATIONS:**
- Async processing patterns
- Database query optimization
- Caching strategies
- Load balancing approaches
- Scaling considerations

Label each component with specific versions and configuration details.
Show deployment boundaries and environment separations.
```

---

## 🎯 Business Logic Architecture Prompt

### **Business Domain & Logic Architecture**

**Use this prompt for business-focused architectural diagrams:**

```
Create a business logic architecture diagram for pharmaceutical intelligence showing:

**BUSINESS DOMAINS:**
- Drug Approval Analytics
- Company Performance Analysis
- Market Intelligence
- Competitive Analysis
- Regulatory Intelligence
- Investment Analysis

**CORE BUSINESS ENTITIES:**
- Drug Approvals (applications, approvals, rejections)
- Pharmaceutical Companies (sponsors, manufacturers)
- Therapeutic Areas (medical categories, market segments)
- Patents and Exclusivity (intellectual property)
- Market Data (sizes, trends, forecasts)

**BUSINESS PROCESSES:**
- Drug Approval Workflow Analysis
- Company Performance Evaluation
- Market Share Calculation
- Competitive Landscape Mapping
- Patent Cliff Analysis
- Generic Opportunity Identification

**KEY PERFORMANCE INDICATORS (KPIs):**
- Approval Success Rates
- Time-to-Market Analysis
- Market Share Metrics
- Competitive Positioning
- R&D Productivity
- Revenue Impact Analysis

**ANALYTICAL WORKFLOWS:**
1. Data Collection → 2. Business Rule Application → 3. KPI Calculation → 
4. Trend Analysis → 5. Competitive Comparison → 6. Insight Generation → 
7. Recommendation Development → 8. Executive Reporting

**BUSINESS INTELLIGENCE LAYERS:**
- Operational Analytics (daily metrics)
- Tactical Analytics (monthly trends)
- Strategic Analytics (yearly forecasts)
- Competitive Intelligence (market positioning)
- Investment Intelligence (opportunity analysis)

**USER PERSONAS:**
- C-Suite Executives (strategic insights)
- Business Analysts (operational metrics)
- Investment Managers (market opportunities)
- Regulatory Affairs (compliance tracking)
- R&D Teams (pipeline analysis)

**DECISION SUPPORT:**
- Market Entry Analysis
- Portfolio Optimization
- Competitive Strategy
- Investment Prioritization
- Risk Assessment

**VALUE CHAIN ANALYSIS:**
- Drug Discovery Impact
- Clinical Trial Insights
- Regulatory Strategy
- Commercial Strategy
- Post-Market Analysis

**BUSINESS METRICS:**
- Revenue Impact ($MM)
- Market Share (%)
- Time Savings (hours)
- Decision Quality (accuracy)
- Risk Reduction (probability)

**REPORTING HIERARCHY:**
Executive Summary → Departmental Reports → Operational Dashboards → 
Detailed Analytics → Supporting Data

Show business value flow from raw data to executive decision-making.
Include business rules, calculations, and decision points.
Map business processes to technical implementations.
```

---

## 📱 User Experience Architecture Prompt

### **User Interface & Interaction Design**

**Use this prompt for UX/UI architecture diagrams:**

```
Create a user experience architecture diagram showing:

**USER PERSONAS:**
- Executive Users (C-suite, board members)
- Business Analysts (market researchers, strategists)
- Data Scientists (quantitative analysts, modelers)
- Operations Users (regulatory affairs, business development)

**USER JOURNEY FLOWS:**
- Executive Dashboard View (high-level KPIs and trends)
- Analyst Deep-dive (detailed analysis and exploration)
- Scientist Model Interaction (prediction and validation)
- Operations Monitoring (real-time updates and alerts)

**INTERFACE COMPONENTS:**
- Navigation and Menu Systems
- Dashboard Layouts and Widgets
- Interactive Charts and Graphs
- Data Filter and Search Interfaces
- Export and Sharing Controls

**INTERACTION PATTERNS:**
- Click-through Analysis (drill-down capabilities)
- Hover Details and Tooltips
- Dynamic Filtering and Sorting
- Real-time Data Updates
- Collaborative Features

**RESPONSIVE DESIGN:**
- Desktop Layout (full feature access)
- Tablet Layout (touch-optimized interactions)
- Mobile Layout (essential features only)
- Cross-platform Consistency
- Accessibility Compliance

**DATA VISUALIZATION HIERARCHY:**
- Executive Summary (key metrics, trends)
- Operational Dashboards (daily/weekly metrics)
- Analytical Workspaces (exploration tools)
- Detailed Reports (comprehensive analysis)
- Export Formats (PDF, Excel, presentations)

**USER WORKFLOW STATES:**
- Login and Authentication
- Dashboard Selection and Customization
- Data Exploration and Analysis
- Insight Discovery and Validation
- Report Generation and Sharing
- Alert Management and Notifications

**INFORMATION ARCHITECTURE:**
- Primary Navigation (main sections)
- Secondary Navigation (sub-categories)
- Contextual Actions (page-specific options)
- Global Search and Filtering
- Help and Documentation Access

**PERSONALIZATION FEATURES:**
- Custom Dashboard Configuration
- Saved Queries and Filters
- Personalized Alerts and Notifications
- User Preferences and Settings
- Collaborative Workspaces

**PERFORMANCE & USABILITY:**
- Fast Loading Times (<2 seconds)
- Intuitive Navigation Patterns
- Clear Visual Hierarchy
- Consistent Design Language
- Error Prevention and Recovery

**ACCESSIBILITY CONSIDERATIONS:**
- Screen Reader Compatibility
- Keyboard Navigation Support
- Color Contrast Compliance
- Font Size and Readability
- Alternative Text for Images

Show user flow paths, interaction touchpoints, and feature priorities for each persona.
Include mobile and desktop interface variations.
Map user goals to interface capabilities.
```

---

## 🔒 Security Architecture Prompt

### **Security & Compliance Architecture**

**Use this prompt for security-focused diagrams:**

```
Create a comprehensive security architecture diagram showing:

**AUTHENTICATION LAYER:**
- User Authentication (Supabase Auth)
- Multi-factor Authentication (MFA)
- Single Sign-On (SSO) Integration
- Session Management
- Password Policies and Rotation

**AUTHORIZATION LAYER:**
- Role-Based Access Control (RBAC)
- Row-Level Security (RLS) in database
- API Endpoint Permissions
- Data Access Controls
- Administrative Privileges

**DATA SECURITY:**
- Encryption at Rest (database encryption)
- Encryption in Transit (TLS/SSL)
- API Key Management
- Database Connection Security
- Sensitive Data Handling

**NETWORK SECURITY:**
- API Gateway Security
- Rate Limiting and DDoS Protection
- CORS Configuration
- Firewall Rules
- VPN Access (if applicable)

**APPLICATION SECURITY:**
- Input Validation and Sanitization
- SQL Injection Prevention
- Cross-Site Scripting (XSS) Protection
- Cross-Site Request Forgery (CSRF) Protection
- Security Headers Implementation

**API SECURITY:**
- API Key Authentication
- JWT Token Management
- Rate Limiting per User/IP
- Request Validation
- Response Sanitization

**MONITORING & AUDIT:**
- Security Event Logging
- Access Audit Trails
- Failed Login Monitoring
- Suspicious Activity Detection
- Compliance Reporting

**COMPLIANCE REQUIREMENTS:**
- Data Privacy (GDPR considerations)
- Healthcare Data Handling
- Industry Security Standards
- Audit Trail Requirements
- Data Retention Policies

**SECURITY ZONES:**
- Public Zone (unauthenticated access)
- User Zone (authenticated users)
- Admin Zone (administrative access)
- System Zone (internal services)
- Data Zone (sensitive data access)

**THREAT MITIGATION:**
- SQL Injection Prevention
- API Abuse Protection
- Data Breach Prevention
- Unauthorized Access Prevention
- Denial of Service Protection

**SECURITY WORKFLOW:**
1. User Access Request → 2. Authentication Verification → 
3. Authorization Check → 4. Data Access Control → 
5. Activity Logging → 6. Continuous Monitoring → 
7. Threat Detection → 8. Incident Response

**VULNERABILITY MANAGEMENT:**
- Regular Security Scanning
- Dependency Vulnerability Checks
- Penetration Testing
- Security Code Reviews
- Incident Response Procedures

Show security boundaries, trust zones, and data sensitivity levels.
Include threat vectors and mitigation strategies.
Map security controls to business requirements.
```

---

## 🎯 How to Use These Prompts

### **For Different Diagramming Tools**

#### **Lucidchart**
1. Copy the relevant prompt
2. Paste into Lucidchart's AI diagram generator
3. Refine and customize the generated diagram
4. Add your specific project details

#### **Draw.io / Diagrams.net**
1. Use the prompt as a reference guide
2. Manually create components based on the prompt structure
3. Follow the suggested layouts and connections
4. Add colors and styling as described

#### **Mermaid (GitHub/GitLab)**
1. Use the prompt structure to create Mermaid syntax
2. Convert architectural components to Mermaid notation
3. Add to your documentation markdown files
4. Version control your diagrams with your code

#### **Microsoft Visio**
1. Use the prompt as a blueprint
2. Create professional enterprise-style diagrams
3. Include detailed technical specifications
4. Export for documentation and presentations

### **Customization Tips**
- **Start with the Master Architecture** prompt for overall system view
- **Use specific prompts** for detailed component views
- **Combine multiple prompts** for comprehensive documentation
- **Adapt terminology** to match your specific implementation
- **Add your branding** and project-specific details

### **Documentation Integration**
- **Save diagrams** in `docs/architecture/` folder
- **Export multiple formats** (PNG, SVG, PDF) for different uses
- **Version control** architectural changes
- **Reference in documentation** with clear explanations

These prompts will help you create **professional, comprehensive architectural documentation** that showcases your system design skills and makes your project portfolio-ready! 🏗️📊

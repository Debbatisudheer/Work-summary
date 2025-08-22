# 💼 Work Summary

## 1. Security Cloud Control (SCC) – Micro Frontend Application
- Worked on **Notification Micro Frontend (MFE)** and **UI Shell (Host) Application**.  
- Integrated micro-frontend apps into the shell application and customized features per requirements.  
- Enhanced **UI/UX using Cisco Magnetic Design System** (pre-defined Cisco components).  
- Implemented **state management, routing, shared libraries, and environment configurations**.  
- Wrote tests with **React Testing Library**, used **Storybook** for component documentation, and configured **webpack, loaders, babel**.  

**Key Topics Covered in React:** Components, Props, State, Hooks, Context, HOCs, Routing, State Management, Fetch API, Providers, bundle.js, Source Maps, .env, .npmrc, Plugins  

**Key Tech:** React.js, Next.js, Storybook, Webpack, Cisco MDS, BootstrapProvider  

---

## 2. Go WebSocket Client & Mock Server
- Developed a **Go WebSocket client** for sending logs, telemetry, and security events to backend systems.  
- Built an **Express.js mock server** to simulate backend APIs, enabling testing and integration without needing the real backend.  

**Key Tech:** Go, WebSocket, Express.js, REST APIs  

---

## 3. Tools Used
- **TablePlus** – Database management (view, query, update, backup MySQL/Postgres/MongoDB).  
- **Postman** – API testing & automation.  
- **JFrog Artifactory** – Artifact storage & distribution across environments.  
- **Cisco Defense Orchestrator (CDO)** – Centralized cloud-based security management platform for firewalls & VPNs.  

---

## 4. Event Collector (Syslog Parsing)
- Enhanced the **Event Collector repo** by modifying Go code to use **comma+space (, ) delimiter** for syslog parsing instead of just comma.  
- Ensured **key-value event parsing** from network devices (firewalls, etc.) without breaking on extra commas.  
- Validated events via **WebSocket client with JWT authentication** and integrated events into the **Cisco CDO portal**.  
- Made multiple feature enhancements in Event Collector as per design requirements.  

**Key Tech:** Go, WebSocket, JWT, Syslog, CDO  

---

## 5. Terraform – Event Collector Infrastructure
- Refactored Terraform deployment using **modularization**:  
  - Split monolithic Terraform codebase into reusable modules (ALB, WAF, Splunk, Datadog, Infra, etc.).  
  - Enabled **independent deployments** for each component → faster, reusable, and scalable.  
- Improved maintainability, testing, and environment reusability (dev, staging, prod).  

**Key Tech:** Terraform, AWS (ALB, WAF, ECS, Infra), Splunk, Datadog  

---

## 6. Jenkins Pipeline Automation
- Designed a **Jenkins pipeline** to automate deployments with Terraform.  
- **Pipeline Stages:**  
  - **Prepare Environment** → AWS credentials, Terraform plugins, env vars.  
  - **Checkout Code** → Fetch commit/branch with Git.  
  - **Deploy Components** → Run `createDeployment.py`, update `overrides.tf.json`, trigger `make plan/deploy`.  
- Reduced deployment errors and enabled selective component deployments.  

**Key Tech:** Jenkins, Terraform, Python (`createDeployment.py`), Bash (.sh), Makefile  

---

## 7. AWS ECS Task Checker
- Built an **AWS Lambda function** to analyze recently stopped ECS tasks.  
- Detected task failures due to **scaling/maintenance vs unexpected errors**.  
- Triggered alerts (**PagerDuty**) for abnormal task stoppages.  

**AWS Components Covered:** EC2, ECS, Lambda, S3, CloudWatch, IAM, Secrets Manager, WAF  

---

## 8. AI/ML – ECS Task Failure Prediction
- Proposed and implemented a **proof-of-concept AI solution** for early ECS task failure prediction.  
- Leveraged **Amazon Lookout for Metrics** with CloudWatch logs + ECS metrics for anomaly detection.  
- Enabled **proactive alerting** and reduced ECS downtime.  

**Key Tech:** AWS Lookout for Metrics, S3, CloudWatch, ECS, AI/ML anomaly detection  

---

## 9. Additional Tools & Integrations
- **Docker** – Containerization of services.  
- **Splunk & Datadog** – Event monitoring, telemetry, observability.  

---

# 📌 Key Technologies Across Projects
- **Languages/Frameworks:** Go, React.js, Next.js, Python, JavaScript  
- **Cloud & Infra:** AWS (ECS, EC2, S3, Lambda, IAM, WAF, CloudWatch), Terraform, Jenkins  
- **DevOps Tools:** Docker, JFrog, Postman, TablePlus, Splunk, Datadog  
- **Frontend Tools:** Storybook, Webpack, React Testing Library, Cisco MDS  
- **Security:** Cisco Defense Orchestrator (CDO), JWT Authentication  


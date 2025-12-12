# Day-1

---

## Introduction to DevOps

### What is DevOps?

DevOps (Development + Operations) is a modern software development approach that emphasizes collaboration, automation, and integration between software developers and IT operations teams. The primary goal is to shorten the development lifecycle and enable continuous delivery of high-quality software.

![Alt Text](img/e404c522-8c6c-429a-b226-f8c98b9c3948.gif)

### Historical Context

**Before DevOps:**
- Development and Operations teams worked in silos
- Release cycles took months or years
- Manual processes led to frequent errors
- Communication was poor between teams
- Blame culture existed when things went wrong

**After DevOps:**
- Teams work collaboratively from the start
- Releases happen multiple times per day
- Automation reduces human errors
- Shared responsibility and accountability
- Focus on continuous improvement

### Core Principles of DevOps

**1. Collaboration**
- Developers, testers, and operations work together
- Shared goals and metrics
- Open communication channels
- Joint planning and decision-making

**2. Automation**
- Automate repetitive manual tasks
- Reduce human errors
- Speed up processes (build, test, deploy)
- Enable faster feedback loops

**3. Continuous Integration (CI)**
- Developers integrate code multiple times per day
- Automated tests run on every code change
- Issues detected early
- Example: Jenkins automatically builds code when pushed to repository

**4. Continuous Deployment (CD)**
- Automated deployment to production environments
- Fast and reliable releases
- Rollback capabilities if issues occur
- Example: Code automatically deployed after passing all tests

**5. Infrastructure as Code (IaC)**
- Infrastructure defined in code (not manual setup)
- Version control for infrastructure
- Reproducible and scalable environments
- Tools: Terraform, Ansible, CloudFormation

**6. Monitoring and Logging**
- Real-time visibility into application performance
- Quick detection of issues
- Data-driven decision making
- Tools: Prometheus, Grafana, ELK Stack

**7. Feedback Culture**
- Regular feedback loops
- Learning from failures
- Continuous improvement mindset
- Retrospectives and reviews

### Benefits of DevOps

| Benefit | Explanation |
|---------|-------------|
| **Faster Time-to-Market** | Reduce time between development and production (from months to days/hours) |
| **Higher Quality** | Automated testing catches issues early |
| **Reduced Risk** | Better monitoring and quick rollback capabilities |
| **Cost Efficiency** | Automation reduces manual work; better resource utilization |
| **Employee Satisfaction** | Reduced toil; focus on meaningful work |
| **Scalability** | Infrastructure as code enables easy scaling |

---

## How IT Company Works

### Organizational Structure

```
┌─────────────────────────────────────────┐
│         IT Company Management            │
├─────────────────────────────────────────┤
│                                         │
│  ┌─────────────┐  ┌──────────────┐    │
│  │Development  │  │   Testing    │    │
│  │   Team      │  │    Team      │    │
│  └─────────────┘  └──────────────┘    │
│                                         │
│  ┌─────────────┐  ┌──────────────┐    │
│  │ Operations  │  │   Project    │    │
│  │   Team      │  │  Management  │    │
│  └─────────────┘  └──────────────┘    │
│                                         │
└─────────────────────────────────────────┘
```

### Department Responsibilities

#### 1. Development Team
**What they do:**
- Analyze client requirements
- Design software architecture
- Write code for features and functionality
- Participate in code reviews
- Fix bugs identified by testers
- Create technical documentation

**Skills Needed:**
- Programming languages (Java, Python, JavaScript, Go, etc.)
- Database design (SQL, NoSQL)
- System design principles
- Version control (Git)
- API development

**Example:** If a client needs an e-commerce website, developers write the code for product catalog, shopping cart, payment integration, etc.

---

#### 2. Testing/QA Team
**What they do:**
- Create test cases based on requirements
- Execute manual and automated tests
- Identify and document bugs
- Verify bug fixes
- Perform performance testing
- Ensure compliance with requirements

**Skills Needed:**
- Test automation (Selenium, TestNG,Postman,sonarqube)
- Manual testing techniques
- SQL for database testing
- API testing (Postman)
- Performance testing tools

**Example:** For the e-commerce website, testers verify that products display correctly, shopping cart calculations are accurate, payment processing works, etc.

---

#### 3. Operations Team
**What they do:**
- Manage servers and infrastructure
- Handle deployment processes
- Monitor application performance
- Manage databases
- Handle backups and disaster recovery
- Ensure system uptime and reliability
- Apply security patches

**Skills Needed:**
- Linux/Unix administration
- Server management
- Network management
- Database administration
- Cloud platforms (AWS, Azure)
- Automations tools (Gir,Docker,K8s,terrform,etc.)

**Example:** Operations team ensures the e-commerce website stays online 24/7, manages database backups, handles traffic spikes during sales, etc.

---

#### 4. Project Management
**What they do:**
- Gather requirements from clients
- Plan project timeline and resources
- Assign tasks to team members
- Track progress
- Manage communication with clients
- Handle risks and issues
- Ensure project stays within budget

**Skills Needed:**
- Agile/Scrum methodologies
- Communication skills
- Leadership
- Risk management
- Budget management

---

### Software Development Lifecycle (SDLC)

A typical IT company follows this process for every project:

**Phase 1: Requirements Gathering**
- Meet with clients to understand needs
- Document functional and non-functional requirements
- Create specifications document
- **Timeline:** 1-2 weeks

**Phase 2: Design**
- Architects design the solution
- Create system architecture diagrams
- Database schema design
- Create technical specifications
- **Timeline:** 1-2 weeks

**Phase 3: Development**
- Developers write code based on design
- Code committed to version control multiple times daily
- Code reviews by senior developers
- **Timeline:** 2-4 weeks (depends on complexity)

**Phase 4: Testing**
- Testers execute test cases
- Report bugs to developers
- Developers fix bugs
- Regression testing (retesting after fixes)
- **Timeline:** 1-2 weeks

**Phase 5: Deployment**
- Prepare production environment
- Deploy application to production
- Smoke testing in production
- **Timeline:** 1 day

**Phase 6: Maintenance & Support**
- Monitor application performance
- Fix issues reported by users
- Release patches and updates
- **Timeline:** Ongoing

### Common Challenges in IT Companies

**1. Slow Release Cycles**
- Testing takes weeks
- Manual deployment processes
- Approval workflows cause delays
- **Solution:** DevOps automation

**2. Poor Communication**
- Silos between teams
- Miscommunication about requirements
- Blame culture when issues occur
- **Solution:** Collaborative tools, shared goals

**3. Manual and Error-Prone Processes**
- Manual testing misses bugs
- Manual deployments cause errors
- Infrastructure setup is repetitive
- **Solution:** Automation and IaC

**4. Scalability Issues**
- Adding servers is time-consuming
- Cannot handle traffic spikes
- **Solution:** Cloud infrastructure, containerization

---

## What is an Application?

### Definition

An **application** (or app) is a software program or set of programs designed to perform specific functions or tasks for end-users, businesses, or organizations.

### Characteristics of Applications

- **Purpose-driven:** Designed to solve specific problems
- **User-centric:** Built with end-users in mind
- **Functional:** Performs specific operations
- **Maintainable:** Can be updated and improved
- **Scalable:** Can handle growth in users/data

### Types of Applications

#### 1. Web Applications
**Definition:** Applications accessed through web browsers using HTTP/HTTPS protocols

**Examples:**
- Gmail (email service)
- Google Docs (document editing)
- Facebook (social media)
- Netflix (video streaming)

**Architecture:**
```
User's Browser → Web Server → Application Server → Database
     (Client)       (Server)        (Business Logic)   (Data)
```

**Advantages:**
- No installation required
- Works on any device with a browser
- Easy to update
- Accessible from anywhere

---

#### 2. Desktop Applications
**Definition:** Applications installed directly on computers (Windows, Mac, Linux)

**Examples:**
- Microsoft Office (Word, Excel, PowerPoint)
- Adobe Photoshop (image editing)
- Visual Studio Code (code editor)
- Slack (communication)

**Advantages:**
- Better performance (local processing)
- Works offline
- Full access to system resources

**Disadvantages:**
- Requires installation on each machine
- Updates need manual installation
- Platform-specific

---

#### 3. Mobile Applications
**Definition:** Applications installed on smartphones and tablets

**Examples:**
- Instagram (social media)
- Uber (ride-sharing)
- WhatsApp (messaging)
- Pokemon Go (gaming)

**Types:**
- **Native Apps:** Built for specific OS (iOS using Swift, Android using Java/Kotlin)
- **Hybrid Apps:** Use web technologies (React Native, Flutter)

**Advantages:**
- Optimized for mobile devices
- Access to device features (camera, GPS, contacts)
- Works offline

---

#### 4. Enterprise Applications
**Definition:** Large-scale applications used by organizations for business operations

**Examples:**
- SAP (enterprise resource planning)
- Salesforce (customer relationship management)
- Oracle (database management)
- Jira (project management)

**Characteristics:**
- Serve thousands of users
- Handle massive amounts of data
- Mission-critical for businesses
- Complex and feature-rich

---

### Application Architecture

#### Monolithic Architecture
**Structure:** Entire application in one large codebase
```
┌────────────────────────────────────────┐
│      Monolithic Application             │
├────────────────────────────────────────┤
│  ┌──────────────────────────────────┐  │
│  │  User Interface (UI)             │  │
│  │  Business Logic                  │  │
│  │  Data Access Layer               │  │
│  │  Database                        │  │
│  └──────────────────────────────────┘  │
└────────────────────────────────────────┘
```

**Pros:** Simple to develop, easy to deploy
**Cons:** Hard to scale, difficult to maintain, one bug affects everything

#### Microservices Architecture
**Structure:** Application broken into small, independent services
```
┌──────────┐  ┌──────────┐  ┌──────────┐
│  User    │  │ Product  │  │ Payment  │
│ Service  │  │ Service  │  │ Service  │
└──────────┘  └──────────┘  └──────────┘
     ↓             ↓              ↓
   DB 1          DB 2           DB 3
```

**Pros:** Scalable, independent deployment, easy to maintain
**Cons:** More complex, requires DevOps expertise

---

### Application Development Lifecycle

**1. Planning**
- Understand client needs
- Define scope and features
- Estimate timeline and resources
- **Duration:** 1-2 weeks

**2. Design**
- UI/UX design (mockups, wireframes)
- System architecture design
- Database design
- API design
- **Duration:** 1-2 weeks

**3. Development**
- Write code for frontend (UI)
- Write code for backend (business logic)
- Integrate different components
- **Duration:** 2-8 weeks (depends on complexity)

**4. Testing**
- Unit testing (individual components)
- Integration testing (components together)
- System testing (entire application)
- UAT (User Acceptance Testing)
- **Duration:** 1-4 weeks

**5. Deployment**
- Prepare production environment
- Deploy application
- Monitor performance
- **Duration:** 1-2 days

**6. Maintenance**
- Fix bugs reported by users
- Add new features
- Improve performance
- **Duration:** Ongoing

---

## Developers vs Testers vs DevOps Engineers

### 1. Developers (Software Engineers)

#### Who are they?
Developers are professionals who write code to build software applications. They transform requirements into functional software.

#### Key Responsibilities
- **Code Development:** Write clean, efficient, maintainable code
- **Feature Implementation:** Build features based on requirements
- **Bug Fixing:** Fix issues reported by testers
- **Code Reviews:** Review peers' code and provide feedback
- **Documentation:** Create technical documentation
- **Optimization:** Improve code performance
- **Collaboration:** Work with testers and operations

#### Skills Required
**Programming Languages:**
- Backend: Java, Python, C++, Go, Node.js
- Frontend: JavaScript, HTML, CSS, React, Angular
- Mobile: Swift, Kotlin, Flutter, React Native

**Other Skills:**
- Database design (SQL, NoSQL)
- API development (REST, GraphQL)
- Design patterns (MVC, Singleton, Factory)
- Version control (Git/GitHub)
- Problem-solving and algorithms

#### Tools & Technologies Used
```
IDEs/Editors:
├── Visual Studio Code
├── IntelliJ IDEA
├── Eclipse
└── Sublime Text

Version Control:
├── Git
├── GitHub
├── GitLab
└── Bitbucket

Databases:
├── MySQL
├── PostgreSQL
├── MongoDB
└── Redis

Frameworks:
├── Spring Boot (Java)
├── Django (Python)
├── React (JavaScript)
└── Laravel (PHP)
```

#### Daily Tasks Example
```
9:00 AM  - Daily standup (15 min)
9:15 AM  - Code new feature for login page
10:30 AM - Code review from senior developer
11:00 AM - Fix comments from code review
12:00 PM - Lunch break
1:00 PM  - Unit testing of login feature
2:00 PM  - Commit code to GitHub
3:00 PM  - Fix bug reported by testers
4:00 PM  - Documentation
5:00 PM  - End of day
```

---

### 2. Testers (QA Engineers)

#### Who are they?
Testers are professionals who verify that software works as intended. They find bugs before users encounter them.

#### Key Responsibilities
- **Test Planning:** Plan testing strategy based on requirements
- **Test Case Design:** Create test cases covering all scenarios
- **Manual Testing:** Execute tests step-by-step
- **Automated Testing:** Write automation scripts
- **Bug Reporting:** Document bugs with detailed information
- **Regression Testing:** Retest after bug fixes
- **Performance Testing:** Test application under load
- **Documentation:** Create test reports and metrics

#### Skills Required
**Testing Knowledge:**
- Black-box testing (test without seeing code)
- White-box testing (test knowing code structure)
- API testing
- Performance/Load testing
- Security testing
- Mobile testing

**Tools & Technologies:**
- Test automation frameworks (Selenium, TestNG)
- Test management tools (TestRail, Zephyr)
- Bug tracking (Jira)
- Performance tools (JMeter, LoadRunner)
- API testing (Postman, REST Assured)

#### Example Test Case
```
Test Case: Login with Valid Credentials
────────────────────────────────────────
Precondition: User is on login page
Steps:
1. Enter valid email in email field
2. Enter valid password in password field
3. Click "Login" button
Expected Result: User logged in, redirected to dashboard
Actual Result: [To be filled during execution]
Status: PASS/FAIL
```

#### Daily Tasks Example
```
9:00 AM  - Daily standup
9:15 AM  - Review new features and requirements
10:00 AM - Create test cases for new login feature
11:00 AM - Execute test cases manually
12:00 PM - Report bugs in Jira
1:00 PM  - Lunch break
2:00 PM  - Retest fixed bugs
3:00 PM  - Execute automation tests
4:00 PM  - Performance testing
5:00 PM  - Test report generation
```

---

### 3. DevOps Engineers

#### Who are they?
DevOps engineers are professionals who bridge the gap between development and operations. They automate and optimize the entire software delivery process.

#### Key Responsibilities
- **CI/CD Pipeline:** Build and maintain automated build/test/deploy pipelines
- **Infrastructure Management:** Manage servers, networks, and cloud resources
- **Containerization:** Deploy applications using Docker/Kubernetes
- **Infrastructure as Code:** Define infrastructure in code
- **Monitoring & Logging:** Monitor application and infrastructure health
- **Security:** Implement security best practices
- **Disaster Recovery:** Ensure backup and recovery procedures
- **Performance Optimization:** Optimize infrastructure and applications
- **Cost Management:** Optimize cloud costs

#### Skills Required
**Core Skills:**
- Linux/Unix administration
- Networking and firewalls
- Cloud platforms (AWS, Azure, GCP)
- Containerization (Docker, Kubernetes)
- CI/CD tools (Jenkins, GitLab CI, GitHub Actions)
- Infrastructure as Code (Terraform, Ansible)
- Scripting (Bash, Python, Go)
- Monitoring tools (Prometheus, Grafana)
- Logging tools (ELK Stack, Splunk)

#### DevOps Tool Stack
```
Planning & Version Control:
├── Git/GitHub/GitLab
├── Jira
└── Confluence

CI/CD:
├── Jenkins
├── GitLab CI/CD
├── GitHub Actions
└── CircleCI

Containerization:
├── Docker
├── Kubernetes
└── Docker Compose

Infrastructure as Code:
├── Terraform
├── Ansible
├── CloudFormation
└── Puppet

Monitoring:
├── Prometheus
├── Grafana
├── ELK Stack
└── Datadog

Cloud Platforms:
├── AWS
├── Google Cloud
└── Microsoft Azure
```

#### DevOps Workflow Example
```
Developer pushes code → GitHub
         ↓
Webhook triggers Jenkins
         ↓
Jenkins pulls code from GitHub
         ↓
Automated Build (compile code)
         ↓
Automated Tests (unit, integration)
         ↓
Code Quality Check (SonarQube)
         ↓
Build Docker Image
         ↓
Push to Docker Registry
         ↓
Deploy to Staging (Kubernetes)
         ↓
Automated Integration Tests
         ↓
Deploy to Production
         ↓
Monitor with Prometheus/Grafana
```

#### Daily Tasks Example
```
9:00 AM  - Daily standup
9:15 AM  - Monitor production dashboards
9:30 AM  - Fix pipeline failure (Jenkins job)
10:30 AM - Write Terraform code for new AWS infrastructure
12:00 PM - Code review for infrastructure changes
1:00 PM  - Lunch break
2:00 PM  - Deploy new version to staging
3:00 PM  - Investigate production issue
4:00 PM  - Optimize Docker image
5:00 PM  - Documentation and knowledge sharing
```

---

### Detailed Comparison

#### 1. Focus & Goals

| Aspect | Developer | Tester | DevOps |
|--------|-----------|--------|--------|
| **Main Focus** | Writing code/features | Finding bugs/quality | Automation/deployment |
| **Goal** | Implement functionality | Ensure quality | Fast & reliable delivery |
| **Mindset** | Build new features | Break features | Optimize processes |
| **Success Metric** | Features delivered | Bugs found | Deployment frequency, speed |

---

#### 2. Timeline & Work Phases

| Phase | Developer | Tester | DevOps |
|-------|-----------|--------|--------|
| **Planning** | Requirements gathering | Test case design | Infrastructure planning |
| **Development** | Code new features | Design tests | Build pipelines |
| **Execution** | Implementation | Test execution | Deploy & monitor |
| **Continuous** | Ongoing coding | Ongoing testing | Always monitoring |

---

#### 3. Interaction with Other Roles

**Developer:**
```
Developers ←→ Testers (report bugs)
   ↓
Testers report bugs → Developers fix
   ↓
DevOps (deployment)
```

**Tester:**
```
Testers ← Requirements (Product Managers)
   ↓
Test Cases ↓
   ↓
Developers (code) → Testers (test)
   ↓
Testers → Developers (bug reports)
   ↓
DevOps (production validation)
```

**DevOps:**
```
Developers (code) → DevOps (automated build/test/deploy)
Testers (testing requirements) ← DevOps (test environments)
Operations (infrastructure) ← DevOps (Infrastructure as Code)
   ↓
Monitors & Alerts
```

---

#### 4. Technologies & Tools

**Developer Tools:**
- IDEs: VS Code, IntelliJ
- Languages: Java, Python, JavaScript
- Databases: MySQL, MongoDB
- Frameworks: Spring, React, Django
- Version Control: Git

**Tester Tools:**
- Automation: Selenium, TestNG, Cypress
- API Testing: Postman, REST Assured
- Performance: JMeter, LoadRunner
- Bug Tracking: Jira
- Test Management: TestRail

**DevOps Tools:**
- CI/CD: Jenkins, GitLab CI
- Containerization: Docker, Kubernetes
- IaC: Terraform, Ansible
- Monitoring: Prometheus, Grafana
- Cloud: AWS, Azure, GCP

---

#### 5. Problem-Solving Approaches

**Developer** - "How do I implement this feature?"
- Analyzes requirements
- Designs solution
- Writes code
- Tests locally
- Commits to version control

**Tester** - "How can I break this feature?"
- Analyzes requirements
- Designs test scenarios
- Creates test cases
- Executes tests
- Reports issues

**DevOps** - "How do I automate this process?"
- Analyzes deployment needs
- Designs pipeline
- Writes automation scripts
- Implements monitoring
- Optimizes performance

---

#### 6. Career Growth Paths

**Developer:**
```
Junior Developer → Senior Developer → Tech Lead → Architect
                                           ↓
                                     Engineering Manager
```

**Tester:**
```
QA Engineer → Senior QA → QA Lead → Test Architect
                               ↓
                         QA Manager
```

**DevOps:**
```
DevOps Engineer → Senior DevOps → DevOps Lead → Infrastructure Architect
                                       ↓
                               DevOps Manager/Engineering Manager
```

---

## Day-2:

## Top Features of Linux
- Open source: source code available and modifiable.
- Stability and reliability: long uptimes for servers.
- Security: strong permission model, SELinux/AppArmor support.
- Performance: efficient resource usage, suitable for servers and embedded systems.
- Package management: apt, yum, pacman for easy software install/updates.
- Variety of distributions: Ubuntu, CentOS, Fedora, Arch, etc.
- Strong networking and server tools: ssh, cron, systemd, iptables/nftables.
- Customizability: kernels, desktop environments, shells.
- Community support and documentation.

---

## Linux Everywhere
- Servers: web, database, mail, and cloud infrastructure.
- Desktops: developer and power-user environments.
- Embedded systems: routers, IoT devices, smart TVs.
- Mobile: Android uses the Linux kernel.
- Containers & orchestration: Docker, Kubernetes run on Linux.
- Supercomputers and scientific computing.

---

## Unlocking Linux Careers
- Roles: System Administrator, DevOps Engineer, Site Reliability Engineer (SRE), Cloud Engineer.
- Typical tasks: server setup, automation, monitoring, troubleshooting, security hardening.
- Entry path: learn CLI, shell scripting, networking, system internals.
- Progression: certification, specialization (containers, cloud, security).

---

## Why AWS Stands Out in the Cloud Market
- Broad service portfolio: compute, storage, database, ML, analytics, serverless.
- Global footprint: many regions and availability zones.
- Mature ecosystem: rich partner network, integrations, marketplace.
- Enterprise features: compliance, security controls, managed services.
- Scale and reliability: proven at large scale for many customers.

---

## Overview of AWS
- Core services:
  - Compute: EC2, Lambda
  - Storage: S3, EBS, EFS
  - Databases: RDS, DynamoDB
  - Networking: VPC, Route 53, CloudFront
  - Management & Monitoring: CloudWatch, CloudTrail
- Billing: pay-as-you-go, reserved and spot instances for cost savings.
- Security: IAM for identity and access control, encryption, compliance.

---

## Customer Success Stories (short examples)
- Netflix: streaming infrastructure on AWS for global scale.
- Airbnb: uses AWS for scalable backend services.
- Spotify: data processing and analytics on AWS services.
- Small startups: rapid prototyping and global rollout without heavy infra investment.

---

## Scalability and Flexibility of Business with AWS
- Auto-scaling: scale compute automatically with demand.
- Managed services: reduce operational overhead (RDS, EKS).
- Global reach: deploy applications close to users.
- Cost controls: budgeting tools, right-sizing, reserved capacity.

---

## Comparing AWS with Competitors
- AWS vs Azure vs GCP:
  - AWS: broadest service set and market maturity.
  - Azure: strong enterprise integrations, Microsoft ecosystem.
  - GCP: strong data/ML offerings and competitive pricing.
- Choice depends on requirements: services, integrations, price, existing vendor relationships.

---

## Why DevOps is a Growing Career Field
- Faster software delivery expectations from businesses.
- Need for automation, reliability, and continuous delivery.
- Cross-functional skillset valuable across industries.
- DevOps practices reduce time-to-market and operational risk.

---

## High Demand for DevOps Professionals
- Employers seek skills in CI/CD, cloud, containers, IaC, monitoring.
- Roles exist in startups to large enterprises and cloud-native companies.
- Remote and hybrid opportunities widely available.

---

## Salary Expectations and Career Growth
- Entry-level: system admin / junior DevOps — varies by region.
- Mid-level: DevOps Engineer / Cloud Engineer — significant salary increase.
- Senior-level: SRE, DevOps Lead, Cloud Architect — higher compensation and leadership roles.
- Salaries depend on region, experience, certifications, and tech stack.

---

## Skills and Expertise in DevOps
- Linux administration and scripting (Bash, Python).
- CI/CD tools: Jenkins, GitHub Actions, GitLab CI.
- Containers & orchestration: Docker, Kubernetes.
- Infrastructure as Code: Terraform, CloudFormation, Ansible.
- Cloud platforms: AWS, Azure, GCP.
- Monitoring & logging: Prometheus, Grafana, ELK.
- Networking, security best practices, and automation.

---

## Certifications and Learning Resources
- AWS: AWS Certified Cloud Practitioner, AWS Solutions Architect.
- DevOps: Certified Kubernetes Administrator (CKA), HashiCorp Terraform Associate.
- Linux: Linux Foundation Certified, CompTIA Linux+.
- Learning resources: official docs, free courses, hands-on labs (cloud free tiers), community tutorials.

---

## The Future of DevOps Careers
- Growing emphasis on SRE practices and platform engineering.
- More automation, AI-assisted operations, and GitOps adoption.
- Need for multi-cloud and security-focused DevOps skills.

---

## Goal to Achieve in CDEC
- Build foundational skills: Linux CLI, shell scripting, basic networking.
- Learn cloud basics (AWS) and core services.
- Practice CI/CD pipelines and container workflows.
- Earn at least one relevant certification (Linux / AWS / Kubernetes).
- Complete hands-on projects and labs to demonstrate practical skills.

---

## Getting Started with Operating Systems

### What is an Operating System (OS)?
- Software that manages computer hardware and provides services to applications and users.
- Acts as an intermediary between user programs and physical hardware.

### Main Responsibilities
- Process management (create, schedule, terminate processes)
- Memory management (allocate/free RAM)
- File system management (read/write, permissions)
- Device management (drivers for hardware)
- Security and access control
- User interface (CLI/GUI)

---

## Different Types of Operating Systems
- Batch OS — Executes jobs in batches (old mainframes).
- Time-Sharing / Multiuser — Many users share CPU time (e.g., Unix).
- Real-Time OS — Deterministic response for embedded systems.
- Distributed OS — Manages distributed resources across networked machines.
- Network OS — Provides network services (file/print sharing).
- Mobile OS — Optimized for phones/tablets (Android, iOS).
- Embedded OS — For appliances and IoT devices (RTOS, Embedded Linux).

---

## How Operating Systems Impact Your Daily Life
- Enable running apps (browsers, email, messaging).
- Manage smartphone operations (calls, notifications, apps).
- Provide security (user accounts, permissions, updates).
- Control home devices (routers, smart TVs) via embedded OS.
- Power cloud servers and web services people use daily.

---

## Windows vs Unix vs Linux

### Ownership and Origin
- Windows: Developed by Microsoft; proprietary.
- Unix: Originated at AT&T Bell Labs (1970s); many commercial variants (AIX, HP-UX).
- Linux: Kernel by Linus Torvalds (1991); open-source, many distributions (Ubuntu, CentOS).

### Cost and Licensing
- Windows: Commercial license; paid for many editions.
- Unix: Commercial licensing for most proprietary flavors.
- Linux: Mostly free/open-source (GPL); some enterprise distributions offer paid support.

### Security and Privacy
- Windows: Larger target for malware; frequent security updates; telemetry in some editions.
- Unix: Historically used in servers; strong POSIX security model.
- Linux: Strong permission model; active patching and community audits; customizable privacy.

### User Interface
- Windows: Graphical, user-friendly GUI; consistent UX.
- Unix: Historically CLI-first; GUIs available (X11, Wayland).
- Linux: Flexible — CLI (bash, zsh) and multiple desktop environments (GNOME, KDE).

---

## What is a Server?
- A server is a computer or program that provides services to other computers (clients) over a network.
- Examples: web server (Apache, Nginx), database server (MySQL, PostgreSQL), file server (Samba).

---

## Desktop OS vs Server OS

Desktop OS
- Optimized for interactive user experience (GUI, multimedia, peripherals).
- Examples: Windows Desktop, macOS, Ubuntu Desktop.
- Focus: user applications, responsiveness.

Server OS
- Optimized for reliability, performance, remote access and headless operation.
- Examples: Windows Server, Ubuntu Server, CentOS, RHEL.
- Focus: network services, concurrency, uptime, security.

Key differences
- GUI presence (server often headless), default services, update cadence, tuning for workloads.

---

## Introduction to Linux
- Linux refers to the kernel; common distributions bundle the kernel with GNU tools and packages.
- Popular distros: Ubuntu, Debian, Fedora, CentOS, Arch.
- Strengths: open-source, flexible, strong server adoption, container & cloud friendly.

Quick commands for students:
- Check kernel and OS:
  - uname -a
  - lsb_release -a  (may require lsb-release package)
- List processes:
  - ps aux | head
  - top or htop
- Disk and filesystems:
  - lsblk
  - df -h

---

## Architecture of Linux — Layered Notes

- Hardware
  - Physical components: CPU, RAM, disk, network cards, peripherals.
  - Provides raw resources that the kernel manages.

- Kernel
  - Core of the OS: device drivers, process scheduler, memory manager, filesystem (VFS), network stack.
  - Exposes system calls as the interface for user-space programs.
  - Runs in kernel space with full hardware access.

- Shell
  - Command-line interface that interprets user commands and scripts (examples: bash, zsh).
  - Acts as a bridge between the user and kernel (invokes system calls, launches processes).
  - Can be used interactively or for automation via scripts.

- Application
  - User-space programs (browsers, editors, daemons, services).
  - Run with limited privileges and use system calls to request kernel services.
  - Isolated from kernel space to protect system stability and security.

- User (User Layer)
  - Humans and user accounts interacting with the system via shell or GUI.
  - Owns and runs applications; subject to permission and access control enforced by kernel.
  - Includes desktop environments and user sessions.

Diagram (simple)
- Hardware ←→ Kernel (drivers, scheduler, memory) ←→ System Calls ←→ User Space (shells, services, apps)

![Alt Text](img/Linux_arch.png)

---

## Simple Learning Exercises
1. Identify your OS:
   - uname -a
   - lsb_release -a
2. Create a file and check permissions:
   - touch ~/testfile && ls -l ~/testfile
3. View running services:
   - systemctl list-units --type=service | head
4. Explore processes:
   - ps aux --sort=-%cpu | head

---

## Quick Summary for Students
- OS manages hardware and provides a platform for apps.
- Types of OS vary by purpose (desktop, server, real-time, embedded).
- Linux is open-source, widely used on servers and in cloud environments.
- Understanding kernel, system calls, filesystem, and user space is key to Linux mastery.


# Day-4

---

## Mastering the Linux Prompt

### Understanding the Linux Command Prompt

The **Linux Command Prompt** (also called the shell prompt or terminal prompt) is the place where you type commands to interact with the Linux system. It's like a conversation with your computer — you type a command, press Enter, and the computer executes it and shows you the result.

#### What is a Prompt?

A prompt is a text indicator that appears on your terminal screen, showing that the system is ready to accept your input. It's a signal saying: "I'm ready for your command!"

#### Example of a Command Prompt:

```bash
student@linux:~$
```

This simple line contains important information. Let's break it down!

---

## Decoding the Structure of the Command Prompt

The standard Linux command prompt has a specific structure. Understanding each part helps you navigate and interact with your system more effectively.

### Standard Prompt Format:

```bash
username@hostname:current_directory$
```

Let's analyze each component:

#### 1. **Username** (`student`)

```bash
student@linux:~$
└─────┘
```

**What it shows:**
- The username of the currently logged-in user
- In this case: `student`

**Different users, different prompts:**
```bash
# When logged in as 'student' user:
student@linux:~$

# When logged in as 'root' user:
root@linux:~#

# When logged in as 'john' user:
john@linux:~$
```

**Important Distinction:**
- Regular users: prompt ends with `$`
- Root user: prompt ends with `#`

---

#### 2. **@ Symbol** (`@`)

```bash
student@linux:~$
       ↑
```

**What it means:**
- Just a separator that means "at"
- Reads as: "student at linux"
- Divides username from hostname

---

#### 3. **Hostname** (`linux`)

```bash
student@linux:~$
         └────┘
```

**What it shows:**
- The name of your computer/server
- Helps identify which machine you're connected to (important when managing multiple servers)

**Examples:**
```bash
# Local computer named 'mycomputer'
student@mycomputer:~$

# Remote server named 'webserver01'
student@webserver01:~$

# Server in cloud
student@aws-prod-server:~$
```

**Why it matters:**
- When working with multiple servers, you always know which one you're on
- Prevents accidental commands on wrong server

---

#### 4. **Colon** (`:`)

```bash
student@linux:~$
              ↑
```

**What it means:**
- Another separator
- Divides hostname from current directory

---

#### 5. **Current Directory** (`~`)

```bash
student@linux:~$
              └─
```

**What it shows:**
- Your current location in the file system
- `~` is a shortcut meaning "home directory"
- Shows where your next command will be executed

**Examples of current directories:**
```bash
# In home directory
student@linux:~$

# In /home/student/Documents
student@linux:~/Documents$

# In /var/log
student@linux:/var/log$

# In root directory
student@linux:/$

# In /etc/nginx
student@linux:/etc/nginx$
```

---

#### 6. **Prompt Symbol** (`$` or `#`)

```bash
student@linux:~$
              ↑
```

**What it shows:**
- `$` = Regular user prompt (limited permissions)
- `#` = Root/superuser prompt (full permissions)

**Examples:**
```bash
# Regular user
student@linux:~$

# Root user
root@linux:~#

# Another regular user
teacher@linux:~$

# System user
www-data@linux:~$
```

---

### Complete Prompt Breakdown Example:

```bash
student@linux:~/Documents$
└─────┘ └────┘ └──────────┘┘
  |       |         |       └─ Prompt symbol ($ = regular user)
  |       |         └─ Current directory (~/Documents)
  |       └─ Hostname (computer name)
  └─ Username (who you are)
```

**What this means:**
- User `student` is logged in
- On computer named `linux`
- Currently in the `Documents` folder inside home directory
- Ready to accept commands

---

### Real-World Prompt Examples:

#### Example 1: Regular User at Home
```bash
john@ubuntu:~$
```
- User: john
- Computer: ubuntu
- Location: home directory
- Permissions: limited (regular user)

---

#### Example 2: Root User in System Directory
```bash
root@ubuntu:/etc/nginx#
```
- User: root
- Computer: ubuntu
- Location: /etc/nginx directory
- Permissions: full (root user)

---

#### Example 3: System User Running Service
```bash
www-data@webserver01:/var/www/html$
```
- User: www-data (web server user)
- Computer: webserver01
- Location: /var/www/html (web files)
- Permissions: limited (system user)

---

#### Example 4: Different User on Different Server
```bash
admin@prod-database:/home/admin$
```
- User: admin
- Computer: prod-database (production server)
- Location: /home/admin (home directory)
- Permissions: limited (but might have sudo access)

---

## Effective Command Prompt Usage: A Step-by-Step Guide

### Step 1: Understanding the Prompt

When you see the prompt, it means:
- The system is ready to accept commands
- Your previous command has finished executing
- You can type a new command

### Step 2: Basic Command Structure

Every command follows this pattern:

```bash
command [options] [arguments]
```

#### Components:

1. **Command** — What you want to do
   ```bash
   ls          ← command to list files
   mkdir       ← command to make directory
   ```

2. **Options** — How to modify the command (usually start with `-`)
   ```bash
   ls -l       ← -l is an option (long format)
   ls -a       ← -a is an option (show all files)
   ls -la      ← combine multiple options
   ```

3. **Arguments** — What to operate on
   ```bash
   ls /home    ← /home is the argument (list this directory)
   mkdir mydir ← mydir is the argument (create this directory)
   ```

---

### Step 3: Typing and Executing Commands

**The Process:**

```bash
1. See prompt: student@linux:~$
2. Type command: ls -l /home
3. Full line: student@linux:~$ ls -l /home
4. Press Enter to execute
5. System runs command and shows output
6. New prompt appears when done
```

**Visual Example:**

```bash
student@linux:~$ ls -l /home
total 24
drwxr-xr-x 5 student student 4096 Dec  5 10:00 student
drwxr-xr-x 3 teacher teacher 4096 Dec  4 09:30 teacher

student@linux:~$ 
↑
New prompt appears - ready for next command
```

---

### Step 4: Command Examples with Explanations

#### Example 1: List Files

```bash
student@linux:~$ ls
Desktop   Documents   Downloads   Music   Pictures   Videos
```

What happened:
- Typed `ls` (list files command)
- Command executed in current directory (~)
- Shows all files and folders in home directory

---

#### Example 2: List Files with Details

```bash
student@linux:~$ ls -l
total 40
drwxr-xr-x  3 student student 4096 Dec  5 10:15 Desktop
drwxr-xr-x  2 student student 4096 Dec  4 15:30 Documents
-rw-r--r--  1 student student  1024 Dec  3 11:20 notes.txt
```

What happened:
- Typed `ls -l` (list with details)
- `-l` option shows:
  - Permissions
  - Owner
  - File size
  - Date/time created

---

#### Example 3: Change Directory

```bash
student@linux:~$ cd Documents
student@linux:~/Documents$
```

What happened:
- Typed `cd Documents` (change directory)
- Moved into Documents folder
- Prompt changed to show new location (`~/Documents`)

---

#### Example 4: Create Directory

```bash
student@linux:~/Documents$ mkdir my_project
student@linux:~/Documents$ ls
my_project
```

What happened:
- Typed `mkdir my_project` (make directory)
- Created new folder called `my_project`
- `ls` shows the new folder exists

---

#### Example 5: Create File

```bash
student@linux:~/Documents$ touch hello.txt
student@linux:~/Documents$ ls -l
-rw-r--r-- 1 student student 0 Dec  5 10:30 hello.txt
```

What happened:
- Typed `touch hello.txt` (create file)
- Created empty file called `hello.txt`
- `ls -l` shows the file with its details

---

### Step 5: Understanding Command Output

After executing a command, you see:
1. **Command output** — Information the command returns
2. **New prompt** — Indicates command finished, ready for next one

```bash
student@linux:~$ pwd
/home/student
↑
Output: your current directory path

student@linux:~$
↑
New prompt appears - command completed
```

---

### Step 6: Error Handling

When you make a mistake, you get an error message:

```bash
student@linux:~$ cd nonexistent_folder
bash: cd: nonexistent_folder: No such file or directory
student@linux:~$
```

What happened:
- Tried to change to folder that doesn't exist
- System shows error message
- Prompt reappears
- You can try again

---

### Step 7: Command History

The system remembers your previous commands:

```bash
student@linux:~$ history
    1  ls
    2  cd Documents
    3  ls -l
    4  mkdir my_project
    5  touch hello.txt
student@linux:~$
```

**How to use history:**
```bash
# See last 10 commands
history 10

# Run a previous command using number
!2          ← runs command #2 (cd Documents)

# Run last command that starts with 'ls'
!ls

# Go through commands with arrow keys
↑ (up arrow)   ← previous command
↓ (down arrow) ← next command
```

---

### Step 8: Using Tab Completion

**Tab Completion** automatically completes your typing:

```bash
# Start typing:
student@linux:~$ cd Doc

# Press Tab, it auto-completes:
student@linux:~$ cd Documents$

# Saves time and prevents typos!
```

**How to use it:**
- Type first few letters of command or filename
- Press Tab key
- System completes it (if unambiguous)
- If multiple matches, press Tab twice to see all options

---

## Making the Command Prompt Your Own: Customization Tips (Advanced Concept)

### What Can You Customize?

You can change how your prompt looks and behaves by editing configuration files.

---

### Understanding the PS1 Variable

The prompt is controlled by a special variable called `PS1` (Prompt String 1).

#### View Current Prompt:

```bash
student@linux:~$ echo $PS1
\u@\h:\w$
```

This shows the prompt template.

---

### Prompt Variables Explained

| Variable | Shows | Example |
|----------|-------|---------|
| `\u` | Username | student |
| `\h` | Hostname | linux |
| `\w` | Current directory | ~/Documents |
| `\d` | Date | Wed Dec  5 |
| `\t` | Time (HH:MM:SS) | 10:30:45 |
| `\T` | Time (12-hour) | 10:30:45 AM |
| `\$` | $ or # symbol | $ (for user) or # (for root) |
| `\n` | New line | (starts on new line) |

---

### Example Customizations

#### Example 1: Simple Colored Prompt

```bash
# Edit the .bashrc file (configuration file)
nano ~/.bashrc

# Find the line with PS1= and change it to:
export PS1="\u@\h:\w\$ "

# Save and reload
source ~/.bashrc
```

#### Example 2: Colored Prompt with Time

```bash
# Add this to ~/.bashrc
export PS1="[\t] \u@\h:\w$ "
```

This shows:
```bash
[10:30:45] student@linux:~/Documents$
```

---

#### Example 3: Prompt with Colors

```bash
# Add to ~/.bashrc (advanced)
export PS1="\e[32m\u@\h\e[0m:\w$ "
```

This makes username green.

---

#### Example 4: Multi-line Prompt

```bash
# Add to ~/.bashrc
export PS1="\u@\h\n\w$ "
```

Shows as:
```bash
student@linux
~/Documents$
```

---

### How to Make Changes Permanent

1. **Open configuration file:**
   ```bash
   nano ~/.bashrc
   ```

2. **Find the PS1 line:**
   ```bash
   # Search for: PS1=
   ```

3. **Edit or add new PS1:**
   ```bash
   export PS1="your_custom_prompt_here"
   ```

4. **Save (Ctrl+O, Enter, Ctrl+X)**

5. **Reload configuration:**
   ```bash
   source ~/.bashrc
   ```

6. **See changes immediately:**
   ```bash
   # Your prompt should now look different!
   ```

---

### Useful Customizations for Students

#### Simple and Professional:
```bash
export PS1="\u@\h:\w$ "
```

#### With Git Branch (if in git directory):
```bash
export PS1="\u@\h:\w\$(git branch 2>/dev/null | grep '^\*' | colrm 1 2) $ "
```

#### With Current Date:
```bash
export PS1="\d \u@\h:\w$ "
```

#### Minimal and Clean:
```bash
export PS1="\w$ "
```

---

## Introduction to Linux Basic Commands

Now that you understand the prompt, let's learn essential Linux commands!

### Command Categories

1. **File and Directory Commands**
2. **Text Commands**
3. **System Information Commands**
4. **File Content Commands**
5. **Help Commands**

---

## Getting Started with the Linux Terminal

### What is the Terminal?

The terminal is the application window where you see the command prompt and type commands. It's your interface to the Linux command line.

### Opening Terminal

#### On Ubuntu/Debian:
- Right-click on desktop → "Open Terminal Here"
- Or press Ctrl+Alt+T
- Or search for "Terminal" in applications menu

#### On Other Systems:
- Find the Terminal or Console application
- Or SSH into a remote Linux server

---

### Terminal vs Prompt

| Term | Meaning |
|------|---------|
| **Terminal** | The application window |
| **Prompt** | The text line where you type |
| **Shell** | The program that interprets commands |
| **Command Line** | Where you type commands |

---

### First Steps in Terminal

When you open terminal:

```bash
student@linux:~$
```

1. You see your prompt
2. Cursor blinks (ready for input)
3. Type your command
4. Press Enter to execute

---

## Essential System Information: Commands and Tools for Linux

### Understanding System Information

System information tells you about your computer: CPU, RAM, disk space, OS version, etc.

---

### Command 1: `uname` — Unix Name

**Purpose:** Display system information

**Basic Usage:**
```bash
student@linux:~$ uname
Linux
```

**Shows:**
- The kernel name (Linux, Darwin for Mac, etc.)

---

**Detailed Information:**
```bash
student@linux:~$ uname -a
Linux ubuntu 5.15.0-84-generic #94-Ubuntu SMP Fri Oct 7 00:24:33 UTC 2022 x86_64 GNU/Linux
```

**Options:**
- `-a` — All information (kernel, hostname, kernel version, processor type)
- `-s` — Kernel name only
- `-r` — Kernel release
- `-v` — Kernel version
- `-m` — Machine hardware name (x86_64, ARM, etc.)

**What each part means:**
```
Linux              ← Kernel name
ubuntu             ← Hostname
5.15.0-84-generic  ← Kernel version
#94-Ubuntu         ← Build number
x86_64             ← Architecture (64-bit processor)
GNU/Linux          ← Operating system
```

---

### Command 2: `lsb_release` — Linux Standard Base Release

**Purpose:** Show Linux distribution information

**Basic Usage:**
```bash
student@linux:~$ lsb_release -a
No LSB modules are available.
Distributor ID: Ubuntu
Release:        20.04
Codename:       focal
```

**Options:**
- `-a` — All information
- `-d` — Distribution description
- `-r` — Release number
- `-c` — Codename

**What it shows:**
- Distributor: Which Linux distribution (Ubuntu, CentOS, etc.)
- Release: Version number (20.04, 22.04, etc.)
- Codename: Code name for that version (focal, jammy, etc.)

---

### Command 3: `whoami` — Who Am I

**Purpose:** Show the current logged-in user

**Usage:**
```bash
student@linux:~$ whoami
student
```

**Shows:**
- Your username

**When to use:**
- Verify which user account you're using
- Especially useful when logged into multiple systems

---

### Command 4: `id` — Identity

**Purpose:** Show user and group IDs

**Basic Usage:**
```bash
student@linux:~$ id
uid=1000(student) gid=1000(student) groups=1000(student),27(sudo),999(docker)
```

**What it shows:**
- `uid` — User ID number (1000)
- `gid` — Group ID number (1000)
- `groups` — All groups you belong to

**Detailed Breakdown:**
```
uid=1000(student)        ← User ID 1000, username is student
gid=1000(student)        ← Primary group ID 1000, group name is student
groups=1000(student)     ← Member of student group
       27(sudo)          ← Member of sudo group (can use sudo)
       999(docker)       ← Member of docker group
```

---

### Command 5: `hostname` — Computer Name

**Purpose:** Show or change the computer's name

**Usage:**
```bash
student@linux:~$ hostname
linux
```

**Shows:**
- Your computer's hostname

**Change hostname (requires sudo):**
```bash
sudo hostname newname
```

---

### Command 6: `pwd` — Print Working Directory

**Purpose:** Show your current directory

**Usage:**
```bash
student@linux:~$ pwd
/home/student
```

**Shows:**
- Your exact location in the file system

**Examples:**
```bash
# In home directory
student@linux:~$ pwd
/home/student

# In Documents folder
student@linux:~/Documents$ pwd
/home/student/Documents

# In system directory
student@linux:/etc$ pwd
/etc
```

---

### Command 7: `ls` — List Directory Contents

**Purpose:** Show files and folders

**Basic Usage:**
```bash
student@linux:~$ ls
Desktop   Documents   Downloads   Music   Pictures   Videos
```

**Common Options:**
```bash
# Long format with details
student@linux:~$ ls -l

# Show hidden files (starting with .)
student@linux:~$ ls -a

# Combined options
student@linux:~$ ls -la

# Show human-readable file sizes
student@linux:~$ ls -lh

# Sort by modification time
student@linux:~$ ls -lt

# Show only directories
student@linux:~$ ls -d */
```

**Output Explanation (ls -l):**
```bash
-rw-r--r-- 1 student student 1024 Dec 5 10:30 file.txt
│  │  │
│  │  └─ Others can read (r)
│  └──── Group can read (r)
└─────── Owner can read/write (rw)
```

---

### Command 8: `df` — Disk Free

**Purpose:** Show disk space usage

**Basic Usage:**
```bash
student@linux:~$ df
Filesystem     1K-blocks    Used Available Use% Mounted on
/dev/sda1      102081528 45032120 52309292  47% /
```

**Better Format:**
```bash
student@linux:~$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda1        98G   45G   50G  47% /
```

**What it shows:**
- `Filesystem` — Storage device name
- `Size` — Total disk space
- `Used` — Space used
- `Avail` — Space available
- `Use%` — Percentage used
- `Mounted on` — Where it's connected

---

### Command 9: `du` — Disk Usage

**Purpose:** Show how much space directories use

**Usage:**
```bash
student@linux:~$ du -sh ~/Documents
2.5G    /home/student/Documents
```

**Shows:**
- Total size of a directory

**Options:**
- `-s` — Summary (total only)
- `-h` — Human-readable (K, M, G)

**Examples:**
```bash
# Size of current directory
student@linux:~$ du -sh .
1.5G    .

# Size of all subdirectories
student@linux:~$ du -sh */
512M    Desktop
1.2G    Documents
256M    Downloads
```

---

### Command 10: `free` — Memory Information

**Purpose:** Show RAM usage

**Usage:**
```bash
student@linux:~$ free -h
              total        used        free      shared  buff/cache   available
Mem:          7.7Gi       2.3Gi       1.2Gi      256Mi       4.2Gi       4.9Gi
Swap:         2.0Gi       0B          2.0Gi
```

**What it shows:**
- `total` — Total RAM installed (7.7 GB)
- `used` — RAM being used (2.3 GB)
- `free` — Available RAM (1.2 GB)
- `buff/cache` — Cache memory (4.2 GB)
- `available` — Usable memory (4.9 GB)

**Swap:**
- Extension of RAM using hard disk
- Used when RAM is full

---

### Command 11: `top` — System Monitor

**Purpose:** Show running processes and system stats

**Usage:**
```bash
student@linux:~$ top
```

**Shows:**
- Running processes
- CPU usage
- Memory usage
- Process IDs
- User running each process

**How to exit:**
- Press `q` to quit

**Key Information:**
- `PID` — Process ID
- `USER` — User running the process
- `%CPU` — CPU usage percentage
- `%MEM` — Memory usage percentage
- `COMMAND` — Program name

---

### Command 12: `ps` — Process Status

**Purpose:** Show running processes (snapshot)

**Basic Usage:**
```bash
student@linux:~$ ps
  PID TTY      STAT   TIME COMMAND
 1234 pts/0    Ss   0:00 bash
 1245 pts/0    R+   0:00 ps
```

**Better Usage:**
```bash
student@linux:~$ ps aux
```

**Shows all processes with details:**
```bash
USER       PID %CPU %MEM    VSZ   RSS TTY STAT START   TIME COMMAND
root         1  0.0  0.1  43896  6908 ?   Ss   10:00   0:05 /sbin/init
student   1234  0.0  0.2  21540  9876 pts/0 Ss 10:05   0:00 bash
student   1245  0.0  0.1  38900  6500 pts/0 R+ 10:30   0:00 ps aux
```

**Useful Options:**
```bash
# Find a specific process
ps aux | grep python

# Sort by CPU usage
ps aux --sort=-%cpu

# Show process tree
ps aux --forest
```

---

### Command 13: `uptime` — System Uptime

**Purpose:** Show how long system has been running

**Usage:**
```bash
student@linux:~$ uptime
 10:30:45 up 5 days, 3:45, 2 users, load average: 0.45, 0.52, 0.48
```

**What it shows:**
- `10:30:45` — Current time
- `up 5 days, 3:45` — System running for 5 days, 3 hours, 45 minutes
- `2 users` — Number of logged-in users
- `load average` — System load (CPU usage)

---

### Command 14: `date` — Current Date and Time

**Purpose:** Show current date and time

**Usage:**
```bash
student@linux:~$ date
Wed Dec  5 10:30:45 UTC 2024
```

**Custom Format:**
```bash
# Show date only
student@linux:~$ date +%Y-%m-%d
2024-12-05

# Show time only
student@linux:~$ date +%H:%M:%S
10:30:45

# Custom format
student@linux:~$ date "+%A, %B %d, %Y"
Wednesday, December 05, 2024
```

---

### Command 15: `which` — Locate Command

**Purpose:** Show where a command is located

**Usage:**
```bash
student@linux:~$ which python
/usr/bin/python

student@linux:~$ which ls
/bin/ls

student@linux:~$ which gcc
/usr/bin/gcc
```

**Shows:**
- The full path to the executable file

---

### Command 16: `man` — Manual Pages

**Purpose:** Get help for any command

**Usage:**
```bash
student@linux:~$ man ls
LS(1)                            User Commands                           LS(1)

NAME
       ls - list directory contents

SYNOPSIS
       ls [OPTION]... [FILE]...

DESCRIPTION
       List information about the FILEs...
```

**How to use:**
- `Space` — Page down
- `q` — Quit
- `/keyword` — Search
- `n` — Next match

**Examples:**
```bash
# Learn about ls command
man ls

# Learn about mkdir
man mkdir

# Learn about file permissions
man chmod
```

---

### Command 17: `type` — Command Type

**Purpose:** Show what type of command it is

**Usage:**
```bash
student@linux:~$ type ls
ls is aliased to `ls --color=auto'

student@linux:~$ type pwd
pwd is a shell builtin

student@linux:~$ type python
python is /usr/bin/python
```

**Shows:**
- If it's an alias
- If it's a built-in shell command
- If it's an external program (and where)

---

## Quick Reference: Essential Commands Summary

```bash
# System Information
uname -a              # Kernel and system info
lsb_release -a        # Linux distribution info
whoami                # Current user
id                    # User and group IDs
hostname              # Computer name
uptime                # System uptime
date                  # Current date and time

# Directory and Files
pwd                   # Print working directory
ls                    # List files
ls -l                 # List with details
ls -la                # List with hidden files
df -h                 # Disk space usage
du -sh                # Directory size

# Memory and Processes
free -h               # Memory usage
top                   # Real-time process monitor
ps aux                # Show all processes
ps aux | grep python  # Find specific process

# Help and Location
which command         # Find command location
man command           # Show command manual
type command          # Show command type
```

---

## Hands-On Exercises for Students

### Exercise 1: Explore Your System

```bash
# 1. Check your username
whoami

# 2. See your user ID and groups
id

# 3. Check your current location
pwd

# 4. See your Linux distribution
lsb_release -a

# 5. Check system uptime
uptime
```

---

### Exercise 2: Check Disk and Memory

```bash
# 1. See disk space
df -h

# 2. Check a specific directory size
du -sh ~/Documents

# 3. Check RAM usage
free -h

# 4. See which processes use most memory
top
```

---

### Exercise 3: Find and Learn About Commands

```bash
# 1. Find where ls command is
which ls

# 2. Get help about ls
man ls

# 3. Find python installation
which python

# 4. List all processes
ps aux | head
```

---

### Exercise 4: Customize Your Prompt

```bash
# 1. See current prompt setting
echo $PS1

# 2. Edit configuration
nano ~/.bashrc

# 3. Find PS1= line and change to:
export PS1="\u@\h:\w\$ "

# 4. Save and reload
source ~/.bashrc

# 5. See your new prompt!
```

---

## Common Command Usage Patterns

### Pattern 1: View Information About System

```bash
student@linux:~$ uname -a
student@linux:~$ lsb_release -a
student@linux:~$ whoami
```

### Pattern 2: Check Resource Usage

```bash
student@linux:~$ df -h
student@linux:~$ du -sh .
student@linux:~$ free -h
student@linux:~$ top
```

### Pattern 3: Monitor Processes

```bash
student@linux:~$ ps aux
student@linux:~$ ps aux | grep python
student@linux:~$ top
```

### Pattern 4: Get Help

```bash
student@linux:~$ man ls
student@linux:~$ which python
student@linux:~$ type python
```

---

## Key Takeaways for Students

1. **Prompt Structure:** `username@hostname:directory$`
   - Shows who you are, where you are, and what machine

2. **Command Execution:** Type command → Press Enter → See output → New prompt

3. **Navigation:** Use `pwd` to see location, `cd` to change location

4. **System Info:** Use commands like `uname`, `df`, `free`, `top` to check system

5. **Getting Help:** Use `man command` to learn about any command

6. **Tab Completion:** Use Tab to auto-complete commands and filenames

7. **Command History:** Use arrow keys or `history` to recall previous commands

8. **Customization:** Edit `~/.bashrc` to customize your prompt and environment

# Day-5


## Delving Deep into the Linux File System — Practical Notes for Students

This chapter teaches everyday file-system operations you will use frequently: how to move around, create and manage files/directories, view and edit file contents, and safely copy/move/delete files. Each section contains commands and simple examples you can try in the terminal.

---

## 1. Navigating the File System

Purpose: find where you are, list contents, and move between folders.

Basic commands
- Print current directory:
  ```bash
  pwd
  # Example output: /home/rajat
  ```
- List files and directories:
  ```bash
  ls
  ls -l        # long listing: permissions, owner, size, date
  ls -la       # include hidden files (those starting with .)
  ls -lh       # human-readable sizes (K, M, G)
  ```
- Change directory:
  ```bash
  cd /path/to/dir
  cd ~         # go to your home directory
  cd -         # go to previous directory
  cd ..        # go up one level (parent)
  ```
- Show tree view (install if needed: apt install tree):
  ```bash
  tree -L 2 ~/projects
  ```
- Quick navigation helpers:
  - `Tab` for auto-completion of filenames and directories.
  - `pushd /path` and `popd` to use a directory stack (helpful when switching contexts).
  - `cd -` returns to the last directory.

Example session:
```bash
pwd                  # /home/rajat
ls -la               # show files, including .bashrc
cd Documents
pwd                  # /home/rajat/Documents
cd ~/projects/myapp
```

---

## 2. File and Directory Management

Create, inspect, rename, change ownership, and set permissions.

- Create directory:
  ```bash
  mkdir mydir
  mkdir -p parent/child/grandchild   # -p creates parents as needed
  ```
- Remove directory:
  ```bash
  rmdir emptydir       # only removes if directory is empty
  rm -r dir_to_remove  # recursive delete (use with care)
  ```
- Create an empty file (or update timestamp):
  ```bash
  touch notes.txt
  ```
- Rename or move files/directories:
  ```bash
  mv oldname.txt newname.txt
  mv ~/downloads/report.pdf ~/documents/  # move file to folder
  ```
- Copy files and directories:
  ```bash
  cp file.txt /path/to/destination/
  cp -r myproject/ ~/backup/myproject/    # copy directory recursively
  ```
- Inspect file or directory metadata:
  ```bash
  stat file.txt
  ls -l file.txt
  ```
- Change permissions:
  ```bash
  chmod 644 file.txt      # rw-r--r--
  chmod +x script.sh      # make executable
  ```
- Change owner and group (requires sudo for other users):
  ```bash
  sudo chown rajat:staff /var/www/html -R
  ```

Safety tip: always `ls` the path before `rm -r`. Use `echo` to preview destructive commands:
```bash
echo rm -rf /some/path
```

---

## 3. Viewing and Editing Files

Quickly read files, follow logs, search inside files, and edit content.

- View entire file:
  ```bash
  cat file.txt
  ```
- Page through long files:
  ```bash
  less /var/log/syslog    # use Space to page, / to search, q to quit
  ```
- Show start or end of file:
  ```bash
  head -n 20 file.txt     # first 20 lines
  tail -n 20 file.txt     # last 20 lines
  tail -f /var/log/syslog # follow new lines in real time
  ```
- Search inside files:
  ```bash
  grep 'ERROR' app.log
  grep -Ri 'TODO' ~/projects
  ```
- Simple edits (text editors):
  - nano (beginner friendly)
    ```bash
    nano ~/projects/notes.md
    ```
  - vim (power user — steeper learning curve)
    ```bash
    vim ~/scripts/deploy.sh
    ```
- Quick text transformations:
  ```bash
  sed -n '1,50p' file.txt         # show lines 1-50
  awk '{print $1, $3}' data.csv   # print columns 1 and 3
  ```

Example: inspect and follow a web server log
```bash
sudo less /var/log/nginx/error.log
# or follow in real time
sudo tail -f /var/log/nginx/error.log
```

Always back up configuration files before editing:
```bash
sudo cp /etc/nginx/nginx.conf /etc/nginx/nginx.conf.bak
sudo nano /etc/nginx/nginx.conf
# after changes:
sudo systemctl reload nginx
```

---

## 4. Copy, Move, and Delete Files — Practical Patterns

Common operations and safer alternatives.

Copying
- Basic copy:
  ```bash
  cp source.txt destination.txt
  ```
- Preserve attributes (mode, timestamps, links):
  ```bash
  cp -a /source/dir /dest/dir
  ```
- Use rsync for large or repeated copies (recommended):
  ```bash
  rsync -avh --progress ~/projects/myapp/ ~/backup/myapp/
  ```

Moving / Renaming
- Move or rename:
  ```bash
  mv file.txt /other/place/
  mv oldname.txt newname.txt
  ```
- Move directory:
  ```bash
  mv ~/downloads/myfolder ~/projects/
  ```

Deleting (be careful!)
- Remove a single file:
  ```bash
  rm filename.txt
  ```
- Remove multiple files:
  ```bash
  rm file1 file2 file3
  ```
- Recursive and force remove (dangerous):
  ```bash
  rm -rf /path/to/dir
  ```
  - Double-check path; avoid running as root unless necessary.

Safer delete workflow
1. List files to confirm:
   ```bash
   ls -la /path/to/dir
   ```
2. Use `trash` / `gio trash` (desktop environments) or move to a temporary folder:
   ```bash
   mkdir -p ~/trash; mv ~/projects/oldproj ~/trash/
   ```
3. When certain, remove permanently.

Example: backup, then remove
```bash
cp -r ~/projects/demo ~/backup/demo-$(date +%F)
rm -rf ~/projects/demo
```

---

## 5. Quick Exercises (Try in your terminal)

1. Navigate and inspect:
   ```bash
   pwd
   ls -la
   cd /tmp
   mkdir -p ~/lab/demo
   ```
2. Create, edit, and view:
   ```bash
   touch ~/lab/demo/notes.txt
   echo "First note" > ~/lab/demo/notes.txt
   cat ~/lab/demo/notes.txt
   nano ~/lab/demo/notes.txt   # add another line, save
   ```
3. Copy and verify:
   ```bash
   cp -a ~/lab/demo ~/lab/demo-backup
   ls -la ~/lab
   ```
4. Safe remove:
   ```bash
   mv ~/lab/demo ~/lab/demo-to-delete
   ls -la ~/lab
   # after confirming contents:
   rm -r ~/lab/demo-to-delete
   ```

---

## 6. Quick Reference Cheat-sheet

Navigation:
- pwd, ls, ls -la, cd, cd -, tree

Create / Remove:
- mkdir -p, rmdir, rm -r (use safely), touch

Inspect:
- stat, ls -l, file, du -sh, df -h

View & Search:
- cat, less, head, tail, tail -f, grep -R

Edit:
- nano, vim, sed, awk

Copy / Move:
- cp, cp -r, cp -a, rsync -avh, mv

Permissions & Ownership:
- chmod, chown, chgrp

Safety:
- Always verify with ls before rm
- Backup config files before editing
- Prefer rsync for large or incremental copies

---

# Day-6



## Mastering the Linux File System Hierarchy

### Mastering the Linux File System — 19 important directories

- / (root)
  - The top of the filesystem tree. All paths start here.
  - Example: ls -ld /

- /bin
  - Essential user binaries (commands) required for single-user mode and for all users (ls, cp, mv).
  - Example: ls -l /bin/ls

- /boot
  - Files required to boot the system: kernel, initramfs, bootloader config.
  - Example: ls -l /boot

- /dev
  - Device files representing hardware and virtual devices (e.g., /dev/sda).
  - Example: ls -l /dev/sda*

- /etc
  - System-wide configuration files and startup scripts.
  - Example: ls -la /etc | head

- /home
  - Users' personal directories (e.g., /home/rajat).
  - Example: ls -la /home

- /lib
  - Shared libraries required by binaries in /bin and /sbin (32-bit systems).
  - Example: ls -l /lib | head

- /lib64
  - 64-bit shared libraries on 64-bit systems.
  - Example: ls -l /lib64 | head

- /media
  - Mount points for removable media (USB CDs) created automatically (GUI systems).
  - Example: ls -la /media

- /mnt
  - Temporary mount point for administrators (manual mounts).
  - Example: sudo mount /dev/sdb1 /mnt; ls /mnt

- /opt
  - Optional add-on application packages (third-party software).
  - Example: ls -l /opt

- /proc
  - Virtual filesystem providing process and kernel information (procfs).
  - Example: cat /proc/cpuinfo

- /root
  - Home directory for the root user (not the same as /).
  - Example: ls -la /root

- /run
  - Runtime data since boot (sockets, pids); volatile.
  - Example: ls -la /run

- /sbin
  - System binaries for administration (fdisk, ifconfig) — usually run by root.
  - Example: ls -l /sbin

- /srv
  - Data for services provided by the system (WWW, FTP data).
  - Example: ls -la /srv

- /sys
  - Virtual filesystem exposing kernel objects and device tree (sysfs).
  - Example: ls -la /sys/class/net

- /tmp
  - Temporary files — world-writable, often cleared at reboot.
  - Example: ls -la /tmp

- /var
  - Variable data: logs (/var/log), mail, spool files, package caches.
  - Example: ls -la /var/log

---

## The Significance of the Linux File System Hierarchy

- Predictability: standard locations make it easy to find binaries, configs, and logs.
- Separation of concerns: isolates user data, system files, runtime data, and optional software.
- Permissions & security: directories have differing default permissions and purposes.
- Maintainability: backups, package management, and recovery are simpler with a consistent layout.

---

## Inside the Linux Root Directory: What You Need to Know

- Root (/) contains mount points and top-level directories — do not store user files directly in /.
- Mounted filesystems (external disks, network mounts) appear at mount points (e.g., /mnt, /media).
- Virtual filesystems (/proc, /sys, /run) are kernel-provided views — read-only or volatile.
- Lost+found: usually present on filesystems formatted with ext{2,3,4}; stores recovered file fragments after fsck.
- Use ls -ld and stat to inspect ownership, perms, and mount points:
  - stat /

---

## Understanding the Functionality of Common Linux Directories (quick guide)

- Binaries: /bin, /sbin, /usr/bin, /usr/sbin
  - User vs system admin tools; /usr/* holds larger collections installed by packages.
- Libraries: /lib, /lib64, /usr/lib
  - Shared code used by binaries.
- Configuration: /etc
  - Centralized system configuration; backup before editing.
- User data: /home, /root
  - Personal files and settings per user.
- Variable & logs: /var (logs, spools, caches)
  - Monitor /var/log for troubleshooting.
- Boot & kernel: /boot
  - Kernel images and bootloader files.
- Devices & runtime: /dev, /proc, /sys, /run
  - Device nodes, process info, kernel object interfaces, and runtime state.
- Optional & service data: /opt, /srv
  - Third-party apps and service-specific content.
- Temporary: /tmp
  - Short-lived files; safe to clean periodically.

---

## Introduction to Linux Shortcuts: Boost Your Efficiency

- ~ (tilde)
  - Shortcut for current user's home directory.
  - Example: cd ~ or cd ~/projects

- / (root)
  - Absolute path starts at root: cd /etc

- . (dot)
  - Current directory. Useful in commands: ./script.sh

- .. (double dot)
  - Parent directory. Example: cd ..

- - (dash)
  - Previous directory. Example: cd -  (switch back)

- Tab completion
  - Press Tab to auto-complete commands, filenames, and paths.

- Ctrl+R (reverse search)
  - Interactive history search to find previous commands.

- Ctrl+C and Ctrl+Z
  - Ctrl+C: kill running foreground process.
  - Ctrl+Z: suspend process (use bg/fg to resume).

- pushd / popd / dirs
  - Directory stack for quick navigation.
  - Example: pushd /var/log; popd

- Aliases
  - Short commands: alias ll='ls -lah'
  - Add to ~/.bashrc to persist.

- Symbolic links
  - Create shortcuts inside filesystem: ln -s /path/to/target ~/shortcut

---

## Hands-on Exercises (short)

1. List top-level directories and permissions:
   - ls -la /
2. Check mount points and disks:
   - lsblk; mount | grep '^/dev'
3. Inspect kernel and process info:
   - cat /proc/cpuinfo | head
4. Use shortcuts:
   - cd ~; mkdir -p ~/lab; pushd /var/log; popd; cd -
5. Create an alias and persist it:
   - echo "alias ll='ls -lah'" >> ~/.bashrc; source ~/.bashrc

---

## Quick Reference (commands)

- Inspect directories:
  - ls -la /path
  - stat /path
- Disk & mounts:
  - lsblk
  - df -h
  - mount
- Virtual fs:
  - ls /proc
  - ls /sys
- Links:
  - ln -s /target /link
- Shortcuts:
  - cd ~, cd -, cd .., Tab, Ctrl+R

---




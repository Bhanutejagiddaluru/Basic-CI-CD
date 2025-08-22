# All You Need to Know About CI/CD

## 📖 For Beginners

Let’s start with a simple story.  
Imagine you are building your **personal portfolio website**.  
Every time you make a small change (update a project, fix a typo, add a new skill), you have to:
- update your resume  
- add a new project  
- fix a typo  

You have to **unpublish the old site**, then **publish the new one**.  

⏳ This cycle wastes time 👉 This takes time.
🚨 Manual steps introduce mistakes 👉 You repeat the same steps again and again.  
⚡ Productivity drops 👉 Mistakes can happen.  


---

## 💡 Solution → CI/CD
That’s why we build **CI/CD** → to save time and reduce mistakes.

<img width="1676" height="263" alt="image" src="https://github.com/user-attachments/assets/012c529d-d6da-4dc1-a2c6-9edd2286ff7b" />

1. CI/CD ?

CI/CD = Continuous Integration / Continuous Delivery (or Deployment).
It’s the process of automating build, test, and release workflows.

2. Continuous Integration (CI)

Highlighted in yellow.

Means: build + test + verify.

Every time code is pushed (new feature, bug fix, etc.), CI automatically:

- Builds the code
- Runs tests
- Verifies everything still works

Goal → catch issues early and keep the main branch stable.

3. Continuous Delivery (CD)

Highlighted in blue.

After CI, the code is always ready to deploy.

But → a human decides when to push it live.

Example: CI pipeline prepares the build, runs tests, stores artifact → engineer presses “Deploy.”

4. Continuous Deployment (CD)

Also highlighted in blue.

After CI, code automatically goes live to users once it passes all tests.

No human button click needed.

Example: Push to main → CI runs → if green, it deploys straight to production.

5. Key Difference

Continuous Delivery → Ready for deployment, but manual release decision.
Continuous Deployment → Deployment is fully automated after tests.

👉 In short:

CI = build + test + verify
CD (Delivery) = package + ready to deploy (manual trigger)
CD (Deployment) = package + deploy + release (automatic to production)



## Level 1
<img width="1051" height="644" alt="image" src="https://github.com/user-attachments/assets/ca245474-4931-43bf-b16f-da04b0544120" />
Image source: ByteByteGo

# CI/CD Pipeline — Stages and Tools

## 🔄 Infinite Loop of DevOps

The pipeline is shown as an infinite loop because **CI/CD is continuous** — it never ends, it repeats with every code change.

---

## 🟣 PLAN
- Tools: **Jira, Confluence**
- Purpose: Plan features, manage tasks, track issues, and document processes.

---

## 🟣 CODE
- Tools: **GitHub, GitLab**
- Purpose: Source control, version management, and collaboration on code.

---

## 🟢 BUILD
- Tools: **Gradle, Bazel, Webpack**
- Purpose: Compile code, build binaries, package applications, bundle frontend assets.

---

## 🔵 TEST
- Tools: **Jest, Playwright, JUnit, Jenkins**
- Purpose: Unit tests, integration tests, end-to-end tests, and pipeline validation.

---

## 🟣 RELEASE
- Tools: **Jenkins, Buildkite**
- Purpose: Package the build, trigger deployment pipelines, prepare for production release.

---

## 🔵 DEPLOY
- Tools: **Docker, Argo, AWS Lambda, Kubernetes, Terraform**
- Purpose: Containerization, orchestration, serverless deployment, and infrastructure automation.

---

## 🟢 OPERATE
- Tools: **Kubernetes, Terraform**
- Purpose: Manage runtime infrastructure, maintain clusters, ensure high availability.

---

## 🟣 MONITOR
- Tools: **Prometheus, Datadog**
- Purpose: Collect metrics, monitor performance, detect errors, and alert on issues.

---

## ✅ Key Insight
- **CI/CD is not just build + deploy.**  
- It is a **full cycle**: Plan → Code → Build → Test → Release → Deploy → Operate → Monitor → back to Plan.  
- Each stage has its own **tools and automation** that keep software delivery **fast, reliable, and repeatable**.






## Level 2

**The difference between high-performing engineering orgs and slow ones? CI/CD maturity.**

Most teams still push code → pray → debug production. Elite teams? **Automated pipelines that ship 100x faster with 90% fewer bugs.**

⚡ **Manual Build/Test/Deploy Overhead** → **Velocity Bottleneck**  
⚡ **CI/CD Automation** → **10x Engineering Productivity** → **DORA Metrics Excellence**

---

🔹 **VERSION CONTROL SYSTEMS + ADVANCED GIT WORKFLOWS**
**Git Hosting Platforms:**
• **GitHub Enterprise** → **GitFlow**, **GitHub Flow**, **Feature Branching**, **Draft PRs**, **CODEOWNERS**, **Branch Protection Rules**
• **GitLab** → **GitLab Flow**, **Merge Request Pipelines**, **GitLab CI Templates**, **Auto DevOps**, **Security Dashboards**
• **Bitbucket** → **Atlassian Bamboo Integration**, **Bitbucket Pipelines**, **Smart Mirroring**, **IP Allowlisting**
• **Azure DevOps Repos** → **TFVC**, **Git Repositories**, **Branch Policies**, **Pull Request Templates**

**Git Workflow Strategies:**
• **GitFlow** → **master/develop/feature/release/hotfix** branches
• **GitHub Flow** → **feature branches** → **pull requests** → **main**
• **GitLab Flow** → **environment branches** → **merge requests**
• **Trunk-based Development** → **short-lived feature branches** → **continuous integration**

---

🔹 **CI/CD ORCHESTRATION ENGINES + ADVANCED FEATURES**
**Cloud-Native CI/CD:**
• **GitHub Actions** → **YAML Workflows**, **Matrix Builds**, **Reusable Actions**, **Composite Actions**, **Environment Secrets**, **OIDC**, **Self-hosted Runners**
• **GitLab CI/CD** → **GitLab Runners**, **Pipeline Templates**, **Auto DevOps**, **Review Apps**, **Feature Flags**, **DAG Pipelines**
• **CircleCI** → **Orbs**, **Workflows**, **Docker Layer Caching**, **Parallelism**, **Test Splitting**, **Dynamic Config**
• **TravisCI** → **Build Matrix**, **Conditional Builds**, **Deployment Providers**

**Enterprise CI/CD:**
• **Jenkins** → **Jenkinsfile**, **Blue Ocean**, **Pipeline as Code**, **Multibranch Pipelines**, **Shared Libraries**, **Build Agents**
• **TeamCity** → **JetBrains**, **Build Configurations**, **Build Chains**, **VCS Triggers**, **Investigation Auto-Assignment**
• **Bamboo** → **Atlassian**, **Deployment Projects**, **Environment Permissions**, **Release Management**

**Cloud Provider CI/CD:**
• **AWS CodePipeline** → **CodeBuild**, **CodeDeploy**, **CodeCommit**, **CodeStar**, **CodeArtifact**, **X-Ray Integration**
• **Azure Pipelines** → **YAML Pipelines**, **Classic Pipelines**, **Multi-stage Pipelines**, **Deployment Jobs**, **Service Connections**
• **Google Cloud Build** → **Cloud Source Repositories**, **Build Triggers**, **Cloud Deploy**, **Skaffold Integration**

**Specialized CI/CD:**
• **Buildkite** → **Agent-based**, **Dynamic Pipelines**, **Test Analytics**
• **Drone** → **Container-native**, **Pipeline Plugins**, **Kubernetes Integration**
• **Tekton** → **Kubernetes-native**, **Cloud Native CI/CD**, **Pipeline Resources**

---

🔹 **BUILD SYSTEMS + ADVANCED PACKAGE MANAGEMENT**
**JVM Ecosystem:**
• **Maven** → **POM.xml**, **Dependency Management**, **Multi-module Projects**, **Maven Central**, **Archetype Generation**, **Site Generation**
• **Gradle** → **Build Scripts**, **Kotlin DSL**, **Build Cache**, **Composite Builds**, **Dependency Locking**, **Build Scans**
• **SBT** → **Scala Build Tool**, **Interactive Shell**, **Incremental Compilation**
• **Leiningen** → **Clojure Build Tool**, **project.clj**, **Plugin System**

**JavaScript/Node.js Ecosystem:**
• **npm** → **package.json**, **npm Scripts**, **npm Workspaces**, **package-lock.json**, **npm Registry**
• **Yarn** → **yarn.lock**, **Yarn Workspaces**, **Plug'n'Play**, **Zero-Installs**, **Berry**
• **pnpm** → **Symlinked node_modules**, **Content-addressable Storage**, **Monorepo Support**

**Build Tools & Bundlers:**
• **Webpack** → **Module Bundling**, **Code Splitting**, **Tree Shaking**, **Hot Module Replacement**, **Module Federation**
• **Rollup** → **ES Modules**, **Bundle Optimization**, **Plugin System**, **Tree Shaking**
• **Vite** → **Hot Module Replacement**, **Build Optimization**, **Plugin Architecture**, **Rollup-based**
• **esbuild** → **Go-based Bundler**, **Ultra-fast Builds**, **TypeScript Support**, **Tree Shaking**
• **SWC** → **Rust-based Compiler**, **TypeScript/JavaScript**, **Faster than Babel**
• **Parcel** → **Zero Configuration**, **Asset Pipeline**, **Hot Reload**
• **Turbopack** → **Vercel**, **Incremental Bundler**, **Rust-based**

**Python Ecosystem:**
• **pip** → **PyPI**, **requirements.txt**, **Virtual Environments**
• **Poetry** → **pyproject.toml**, **Dependency Resolution**, **Virtual Environment Management**
• **Pipenv** → **Pipfile**, **Automatic Virtual Environments**
• **Conda** → **Anaconda**, **Environment Management**, **Cross-language Packages**

**Go Ecosystem:**
• **Go Modules** → **go.mod**, **go.sum**, **Module Proxy**, **Semantic Versioning**
• **Go Build** → **Cross-compilation**, **Build Tags**, **Linking**

**Rust Ecosystem:**
• **Cargo** → **Cargo.toml**, **Crates.io**, **Workspaces**, **Build Scripts**

**.NET Ecosystem:**
• **NuGet** → **packages.config**, **PackageReference**, **Package Management**
• **MSBuild** → **Project Files**, **Targets**, **Properties**
• **dotnet CLI** → **Project Templates**, **Package Management**, **Build/Test/Publish**

---

🔹 **ARTIFACT REPOSITORY MANAGEMENT + REGISTRY ECOSYSTEMS**
**Universal Repositories:**
• **JFrog Artifactory** → **Universal Repository**, **Binary Management**, **Xray Security**, **Build Info**, **AQL Queries**
• **Sonatype Nexus** → **Repository Manager**, **Component Intelligence**, **Vulnerability Scanning**, **Lifecycle Management**

**Language-Specific Registries:**
• **npm Registry** → **JavaScript/Node.js**, **Scoped Packages**, **Private Registries**
• **PyPI** → **Python Package Index**, **Wheel Distribution**, **Test PyPI**
• **Maven Central** → **Java/JVM**, **OSSRH**, **PGP Signatures**
• **Crates.io** → **Rust Packages**, **Semantic Versioning**
• **NuGet Gallery** → **.NET Packages**, **Symbol Packages**

**Cloud Provider Registries:**
• **GitHub Packages** → **npm**, **Docker**, **Maven**, **NuGet**, **RubyGems**
• **AWS CodeArtifact** → **Package Management Service**, **Upstream Repositories**
• **Azure Artifacts** → **Universal Packages**, **Feed Management**, **Upstream Sources**
• **Google Artifact Registry** → **Container Images**, **Language Packages**, **Regional Repositories**

**Container Registries:**
• **Docker Hub** → **Public Registry**, **Official Images**, **Automated Builds**, **Vulnerability Scanning**
• **Amazon ECR** → **Private Registry**, **Vulnerability Scanning**, **Lifecycle Policies**, **Cross-region Replication**
• **Google Container Registry (GCR)** → **gcr.io**, **Artifact Registry Migration**
• **Azure Container Registry (ACR)** → **Geo-replication**, **Content Trust**, **Helm Chart Support**
• **Quay.io** → **Red Hat**, **Security Scanning**, **Robot Accounts**
• **Harbor** → **Open Source**, **Vulnerability Scanning**, **Notary Integration**

---

🔹 **COMPREHENSIVE TESTING AUTOMATION FRAMEWORKS**
**Unit Testing Frameworks:**
• **Java**: **JUnit 5**, **TestNG**, **Mockito**, **AssertJ**, **Hamcrest**
• **.NET**: **NUnit**, **MSTest**, **xUnit.net**, **Moq**, **FluentAssertions**
• **Python**: **PyTest**, **unittest**, **nose2**, **mock**, **pytest-cov**
• **JavaScript/Node.js**: **Jest**, **Mocha**, **Jasmine**, **Vitest**, **Sinon.js**
• **Go**: **testing package**, **Testify**, **GoMock**, **Ginkgo**
• **Rust**: **built-in test framework**, **quickcheck**, **proptest**

**Integration Testing:**
• **Spring Boot Test** → **@SpringBootTest**, **TestContainers**, **MockMvc**
• **TestContainers** → **Docker-based Testing**, **Database Testing**, **Message Queue Testing**
• **WireMock** → **HTTP Service Mocking**, **Stubbing**, **Request Matching**
• **Postman Newman** → **API Testing**, **Collection Runner**, **Environment Variables**
• **REST Assured** → **Java REST API Testing**, **BDD-style**, **JSON/XML Validation**

**End-to-End Testing:**
• **Selenium WebDriver** → **Browser Automation**, **Grid**, **Page Object Model**
• **Cypress** → **JavaScript E2E**, **Time Travel**, **Real-time Reloads**
• **Playwright** → **Microsoft**, **Cross-browser**, **Auto-wait**, **Mobile Testing**
• **WebDriverIO** → **Next-gen WebDriver**, **Sync/Async**, **Mobile Testing**
• **Puppeteer** → **Chrome DevTools Protocol**, **Headless Chrome**
• **TestCafe** → **No WebDriver**, **JavaScript/TypeScript**, **Cross-browser**

**API Testing Specialized:**
• **Karate DSL** → **BDD-style API Testing**, **JSON/XML**, **Parallel Execution**
• **Pact** → **Consumer-driven Contract Testing**, **Provider Verification**
• **Insomnia** → **GraphQL/REST Testing**, **Environment Management**
• **Bruno** → **Open Source API Client**, **Git-friendly**
• **HTTPie** → **Command-line HTTP Client**, **JSON Support**

**Performance & Load Testing:**
• **Apache JMeter** → **GUI/Command-line**, **Protocol Support**, **Distributed Testing**
• **Gatling** → **Scala-based**, **High Performance**, **Real-time Metrics**
• **K6** → **JavaScript**, **Developer-centric**, **Cloud Integration**
• **Artillery** → **Node.js**, **WebSocket/Socket.io**, **Real-time Metrics**
• **Locust** → **Python**, **Distributed**, **Web UI**
• **NBomber** → **.NET**, **C#/F#**, **Cluster Support**

**Security Testing:**
• **OWASP ZAP** → **Web Application Security**, **Passive/Active Scanning**, **API Testing**
• **Snyk** → **Vulnerability Scanning**, **License Compliance**, **Container Scanning**
• **Checkmarx** → **Static Application Security Testing (SAST)**, **Code Analysis**
• **Veracode** → **Static/Dynamic Analysis**, **Software Composition Analysis**
• **SonarQube** → **Code Quality**, **Security Hotspots**, **Technical Debt**
• **Bandit** → **Python Security Linting**
• **ESLint Security Plugin** → **JavaScript Security Rules**

**Mobile Testing:**
• **Appium** → **Cross-platform Mobile Automation**, **WebDriver Protocol**
• **Espresso** → **Android UI Testing**, **Google**
• **XCTest** → **iOS Testing Framework**, **Apple**
• **Detox** → **React Native E2E Testing**

---

🔹 **CODE QUALITY + ADVANCED STATIC ANALYSIS**
**Multi-language Analysis:**
• **SonarQube** → **Code Coverage**, **Technical Debt**, **Security Hotspots**, **Quality Profiles**, **Quality Gates**
• **CodeClimate** → **Maintainability**, **Test Coverage**, **Duplication Detection**
• **Codacy** → **Code Quality**, **Security**, **Coverage Tracking**

**Language-Specific Linters:**
• **JavaScript/TypeScript**: **ESLint** → **Airbnb Config**, **Prettier Integration**, **TypeScript ESLint**
• **Python**: **Pylint**, **Flake8**, **Black** (formatter), **isort** (import sorting)
• **Java**: **Checkstyle** → **Google/Sun Conventions**, **PMD** → **Copy-Paste Detection**, **SpotBugs** → **Bug Detection**
• **Go**: **golint**, **go vet**, **gofmt**, **goimports**
• **Rust**: **Clippy**, **rustfmt**
• **.NET**: **StyleCop**, **FxCop Analyzers**, **EditorConfig**

**Code Formatting:**
• **Prettier** → **JavaScript/TypeScript/CSS/HTML**, **Opinionated Formatter**
• **Black** → **Python Code Formatter**, **Uncompromising**
• **gofmt** → **Go Standard Formatter**
• **rustfmt** → **Rust Code Formatter**

**Dependency Analysis:**
• **OWASP Dependency-Check** → **Vulnerability Scanning**
• **Snyk** → **Dependency Vulnerabilities**, **License Compliance**
• **WhiteSource/Mend** → **Open Source Security**, **License Compliance**
• **Dependabot** → **GitHub**, **Automated Dependency Updates**

---

🔹 **CONTAINERIZATION + ADVANCED REGISTRY MANAGEMENT**
**Container Runtimes & Tools:**
• **Docker** → **Dockerfile**, **Multi-stage Builds**, **BuildKit**, **Docker Compose**, **Docker Swarm**
• **Podman** → **Daemonless Container Engine**, **Rootless Containers**, **Pod Management**
• **Buildah** → **OCI Container Building**, **Scriptable Builds**
• **containerd** → **Container Runtime**, **Kubernetes CRI**
• **CRI-O** → **Kubernetes Container Runtime**, **OCI Compliant**

**Container Build Tools:**
• **Docker BuildKit** → **Concurrent Builds**, **Build Cache**, **Multi-platform**
• **Kaniko** → **Container Builds in Kubernetes**, **No Docker Daemon**
• **img** → **Standalone Container Builds**, **Rootless**
• **Buildpacks** → **Cloud Native Buildpacks**, **Auto-detection**

**Container Security:**
• **Twistlock/Prisma Cloud** → **Container Security Platform**, **Runtime Protection**
• **Aqua Security** → **Cloud Native Security**, **Image Scanning**
• **Sysdig Secure** → **Runtime Security**, **Compliance**
• **Anchore** → **Container Image Analysis**, **Policy Engine**
• **Clair** → **Vulnerability Scanner**, **Static Analysis**

**Registry Management:**
• **Harbor** → **Open Source Registry**, **Vulnerability Scanning**, **Replication**
• **Portus** → **Authorization Service**, **Web UI for Docker Registry**
• **Dragonfly** → **P2P Distribution**, **Image Distribution**

---

🔹 **CONTAINER ORCHESTRATION + KUBERNETES ECOSYSTEM**
**Kubernetes Core:**
• **Kubernetes** → **Deployments**, **Services**, **Ingress**, **StatefulSets**, **DaemonSets**, **Jobs**, **CronJobs**
• **kubectl** → **Command-line Tool**, **Resource Management**
• **kubeconfig** → **Cluster Configuration**, **Context Switching**

**Kubernetes Package Management:**
• **Helm** → **Package Manager**, **Chart Templates**, **Release Management**, **Hooks**, **Values**
• **Kustomize** → **Configuration Management**, **Overlays**, **Patches**
• **Jsonnet** → **Data Templating Language**, **Kubernetes Manifests**

**Kubernetes Distributions:**
• **OpenShift** → **Red Hat Enterprise Kubernetes**, **Source-to-Image**, **Developer Tools**
• **Rancher** → **Multi-cluster Management**, **RKE2**, **Fleet GitOps**
• **Tanzu** → **VMware**, **Kubernetes Platform**, **Application Catalog**
• **EKS** → **AWS Managed Kubernetes**, **Fargate**, **Node Groups**
• **GKE** → **Google Kubernetes Engine**, **Autopilot**, **Workload Identity**
• **AKS** → **Azure Kubernetes Service**, **Virtual Nodes**, **Pod Identity**

**Service Mesh:**
• **Istio** → **Traffic Management**, **Security**, **Observability**, **Envoy Proxy**
• **Linkerd** → **Lightweight Service Mesh**, **Rust-based**, **Zero-config**
• **Consul Connect** → **HashiCorp**, **Service Discovery**, **Secure Communications**
• **Open Service Mesh (OSM)** → **Microsoft**, **SMI Compliant**

**Alternative Orchestrators:**
• **Docker Swarm** → **Native Docker Orchestration**, **Overlay Networks**
• **Nomad** → **HashiCorp Orchestrator**, **Multi-datacenter**, **Flexible Workloads**
• **Apache Mesos** → **Cluster Manager**, **Marathon Framework**

---

🔹 **INFRASTRUCTURE AS CODE + ADVANCED CONFIGURATION MANAGEMENT**
**Infrastructure Provisioning:**
• **Terraform** → **HCL**, **State Management**, **Providers**, **Modules**, **Workspaces**, **Remote State**
• **Pulumi** → **TypeScript/Python/Go/C#**, **Cloud Engineering Platform**, **Stack Management**
• **AWS CloudFormation** → **JSON/YAML Templates**, **Stack Management**, **Drift Detection**
• **Azure Resource Manager (ARM)** → **Bicep**, **Template Deployment**, **Resource Groups**
• **Google Cloud Deployment Manager** → **YAML/Python Templates**, **Declarative Configuration**

**Cloud Development Kits:**
• **AWS CDK** → **TypeScript/Python/Java**, **High-level Constructs**, **CloudFormation**
• **Azure CDK** → **Bicep**, **ARM Template Generation**
• **GCP CDK** → **Cloud Foundation Toolkit**, **Terraform Modules**

**Configuration Management:**
• **Ansible** → **Playbooks**, **Inventory Management**, **Agentless**, **Tower/AWX**
• **Chef** → **Cookbooks**, **Recipes**, **InSpec**, **Chef Server**
• **Puppet** → **Manifests**, **Resource Abstraction Layer**, **PuppetDB**
• **SaltStack** → **Salt States**, **Event-driven Automation**, **Pillars**

**Policy as Code:**
• **Open Policy Agent (OPA)** → **Rego Language**, **Policy Engine**
• **Gatekeeper





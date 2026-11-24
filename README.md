# Rajesh Dhanishetty

**Software Engineer — Azure cloud, reliability engineering, security governance, and applied AI.**

I build and operate Azure services at Microsoft, working through BrickRed Systems: on-call incident response and reliability work for a large-scale data platform, and infrastructure work on Azure Chaos Studio. Recent results: cut regional health-validation costs by ~70%, and eliminated stored credentials from deployment workloads by moving them to managed identities.

10+ years of engineering across automotive and aerospace product development, now working full-time on Azure cloud, DevOps and reliability engineering. Outside work I build end-to-end Azure and AI projects, listed below.

---

### What I work on

- **Incident response & reliability** — on-call for a large-scale data pipeline platform: triaging incidents with KQL and Application Insights, root-causing failures across storage and analytics layers, and tracing noisy alerts to their configuration to cut alert fatigue
- **Security & governance** — subscription-scoped Azure Policy with `DeployIfNotExists` remediation that moves Cosmos DB and Storage Accounts off local-authorization access, fixing existing production resources without redeployment
- **Keyless infrastructure** — migrated deployment-script workloads off stored credentials to managed identity authentication
- **Cost optimization** — replaced high-cost chaos experiments with a lightweight Azure Chaos timed-delay design in Bicep, cutting regional validation costs by ~70%
- **Observability** — retired noisy legacy synthetic monitors and built OpenTelemetry-based availability and failure monitors to replace them
- **Regional expansion** — capacity and quota planning, feature-flagged phased rollouts, and a reusable runbook for building out a new Azure region

---

### Projects

#### [Azure-Cloud-AI](https://github.com/dhanishetty/Azure-Cloud-AI)

An AI platform on Azure, built to show how I design, deploy and operate a real workload. The RAG app (upload a PDF, ask questions, get answers with page citations) runs on **AKS**, is deployed entirely by **GitHub Actions** using OIDC, builds its infrastructure from **Bicep**, and reaches Storage, AI Search and Azure OpenAI with **managed identity** instead of keys. Also built: live YouTube chat sentiment, topic modeling, and a Prometheus / Grafana / Alertmanager monitoring stack, tested in Docker.

`AKS` · `Bicep` · `GitHub Actions` · `Workload Identity` · `Azure OpenAI` · `Azure AI Search` · `FastAPI` · `React` · `Prometheus` · `Grafana`

The cluster is torn down between sessions to save cost, so there is no always-on demo. The repo documents how I built it, step by step, including the problems I hit.

#### [incident-triage-agents](https://github.com/dhanishetty/incident-triage-agents)

A team of eight AI agents that triages an Azure incident. An Azure Monitor alert wakes a supervisor, Logs, Metrics and Change agents query in parallel, a Diagnosis agent names the likely root cause, a Remediation agent proposes a fix, and a person approves before anything runs. A Postmortem agent files the report to Azure DevOps Boards. Includes a demo environment you can break on demand, so the agents investigate real logs, metrics and change history.

`LangGraph` · `FastAPI` · `React` · `Azure Monitor` · `Azure OpenAI` · `Docker`

Early stage: the agent graph runs end to end in Docker. The Azure connectors are built and tested against fakes, and a run on a real subscription is next.

---

### AI and machine learning

| Repository | What's in it |
|---|---|
| **[AI-Engineering-LLMs](https://github.com/dhanishetty/AI-Engineering-LLMs)** | LLM fine-tuning across five task types (LoRA / QLoRA / full), each taken training → adapter merging → evaluation, with adapters and merged models published on [Hugging Face](https://huggingface.co/dhanishetty). Plus Azure AI Services, OpenAI API apps, NLP and classical ML |
| **[AI-Computer-Vision](https://github.com/dhanishetty/AI-Computer-Vision)** | YOLOv8 detection, tracking and zone counting; segmentation and gesture recognition; OpenCV fundamentals; streaming filter pipelines with OpenFilter |
| **[trail-runner](https://github.com/dhanishetty/trail-runner)** | A 3D rolling-ball game you steer with your body: MediaPipe Pose reads the webcam, Ursina (Panda3D) renders the forest trail, packaged as a Windows executable with PyInstaller |

### Study notes

**[Azure](https://github.com/dhanishetty/Azure)** — notes and labs from my Azure study: AKS, Bicep and ARM templates, CI/CD, and chaos engineering with Azure Chaos Studio.

---

### What I work with

**Cloud & platform** — Azure, AKS, Azure Monitor, Azure Chaos Studio, Azure DevOps

**Infrastructure as code** — Bicep, ARM templates

**CI/CD** — Azure DevOps Classic and YAML pipelines, Ev2 safe deployment, GitHub Actions

**Reliability & observability** — OpenTelemetry, KQL / Azure Data Explorer, Application Insights, Prometheus, Grafana, synthetic monitoring, alerting, incident management

**Governance & security** — Azure Policy, managed identities, Workload Identity, Microsoft Entra, Azure RBAC

**Data & containers** — Cosmos DB, Azure Storage, Kubernetes, Docker

**AI / ML** — Azure OpenAI, Azure AI Search (RAG), LangGraph, LoRA & QLoRA fine-tuning, Hugging Face Transformers & PEFT, Weights & Biases, YOLOv8, OpenCV

**Languages** — C#, Python, TypeScript, PowerShell, Bash, SQL, YAML

---

### Certifications

Microsoft Certified: Azure Fundamentals · Azure Developer Associate · Azure Administrator Associate

---

### Elsewhere

[LinkedIn](https://www.linkedin.com/in/rajeshdhanishetty/) · [Hugging Face](https://huggingface.co/dhanishetty) · dhanishetty@gmail.com

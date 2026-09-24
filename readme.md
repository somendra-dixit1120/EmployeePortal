# EmployeePortal

## 🚀 Project Overview
EmployeePortal is an ASP.NET Core application integrated with a fully automated Continuous Integration (CI) pipeline using Azure DevOps. 

## 🛠️ CI/CD & DevOps Infrastructure
* **Version Control:** Managed through Git, including branch synchronization and merge conflict resolution.
* **Automated CI Pipeline:** Configured `azure-pipelines.yml` to automatically restore dependencies, build the .NET project, and publish artifacts triggered by commits to the repository.
* **Pipeline Management:** Successfully transitioned from UI-based classic pipelines to modern YAML-based infrastructure.

## ⚙️ Azure DevOps Self-Hosted Agent
* **Agent Setup:** Deployed a local Windows self-hosted agent to securely build and process the application code.
* **Background Service Migration:** Successfully upgraded the agent from a manual terminal process (`run.cmd`) to a **permanent background Windows Service** (`vstsagent`). The agent now boots automatically with the system and continuously listens for Azure DevOps pipeline triggers without requiring an active command prompt session.

## 🔒 DevSecOps (Roadmap)
* Local environment configured for secret scanning using **GitLeaks**.
* Future pipeline enhancements include integrating **SonarCloud** for automated Static Application Security Testing (SAST).
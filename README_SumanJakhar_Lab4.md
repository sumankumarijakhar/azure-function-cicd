# Azure Function CI/CD Pipeline - Lab 4

## Student Name: Suman Kumari Jakhar  
## Course: Cloud DevOps / Azure Pipelines Lab  
## Submission Date: August 2025

---

## 🔧 Project Overview

This project demonstrates a CI/CD pipeline setup using Azure DevOps that builds, tests, and simulates deployment of a simple Azure Function App written in C#.

Due to limited permissions in the school-provided Azure subscription, the real deployment to Azure Function App is simulated in the pipeline.

---

## 🗂️ Repository Structure

```
azure-function-cicd/
│
├── AzureFuncDemo/                # Function App code (C#)
│   ├── HelloFunction.cs         # Main HTTP trigger
│   └── host.json                # Host config
│
└── .azure-pipelines.yml         # CI/CD Pipeline definition
```

---

## 🚀 Pipeline Stages

The pipeline consists of 3 stages defined in YAML:

### ✅ Build Stage
- Installs .NET SDK
- Restores dependencies
- Builds the function project using `dotnet build`

### ✅ Test Stage
- Simulated test execution using a placeholder `echo` command
- Intended to represent `dotnet test` or other test framework

### ✅ Deploy Stage (Mocked)
- Deployment to Azure is skipped due to lack of access
- Outputs a mock deployment message

---

## 🔗 Resources Used

- GitHub (for source control)
- Azure DevOps (for CI/CD pipeline)
- Azure Functions Core Tools (.NET)
- Azure Portal (attempted deployment)

---

## ⚠️ Notes

- The actual deployment to Azure could not be completed because of permission restrictions on the school Azure account.
- A free parallelism request was submitted to Microsoft as per lab instructions to allow the build agents.
- The pipeline YAML was updated to simulate deployment to demonstrate the workflow.

---

## ✅ Links

- **GitHub Repo:** [azure-function-cicd](https://github.com/sumankumarijakhar/azure-function-cicd)
- **Azure DevOps Pipeline:** Accessible through the `FunctionCICDProject` in Azure DevOps

---

## 📸 Screenshots

Screenshots of pipeline stages and error messages are included in the final submission PDF.

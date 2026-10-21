# DevOps_Terraform 🚀

A hands-on repository documenting my journey into **DevOps, Infrastructure as Code (IaC), and AWS automation using Terraform**.

This repository contains practical exercises, configuration files, and infrastructure provisioning examples to understand how cloud infrastructure can be created, managed, and automated using code.

## 📌 Objectives

- Learn Terraform fundamentals and HashiCorp Configuration Language (HCL).
- Provision and manage AWS infrastructure using Infrastructure as Code.
- Understand Terraform providers, resources, variables, outputs, and state.
- Practice infrastructure planning, deployment, and destruction.
- Explore reusable configurations and modular infrastructure design.
- Develop practical DevOps skills through hands-on implementation.

## 🛠️ Tech Stack

- **Cloud Provider:** Amazon Web Services (AWS)
- **Infrastructure as Code:** Terraform
- **Configuration Language:** HCL
- **Cloud CLI:** AWS CLI
- **Version Control:** Git and GitHub
- **Environment:** Windows / WSL Ubuntu

## 📂 Repository Structure

```text
Devops_Terraform/
├── README.md
├── main.tf
├── provider.tf
├── variables.tf
├── outputs.tf
├── terraform.tfvars.example
└── .gitignore
```

*Note: The structure above is a suggested layout. Adjust it to match the actual files in this repository.*

## ⚙️ Prerequisites

Before getting started, ensure you have:

- An AWS account with the necessary IAM permissions.
- Terraform CLI installed.
- AWS CLI installed and configured.
- Git installed.
- Basic familiarity with Linux commands and cloud computing.

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/anukritigupta07/Devops_Terraform.git
cd Devops_Terraform
```

### 2. Configure AWS Credentials

Configure your AWS CLI credentials using an appropriate IAM identity:

```bash
aws configure
```

Verify your AWS identity:

```bash
aws sts get-caller-identity
```

**Security note:** Never commit AWS access keys, secret keys, session tokens, or other credentials to GitHub.

### 3. Initialize Terraform

```bash
terraform init
```

This initializes the working directory and downloads the required provider plugins.

### 4. Validate the Configuration

```bash
terraform fmt -recursive
terraform validate
```

These commands format Terraform files and check the configuration for errors.

### 5. Preview Infrastructure Changes

```bash
terraform plan
```

Review the proposed changes before creating or modifying any AWS resources.

### 6. Deploy Infrastructure

```bash
terraform apply
```

Review the execution plan and confirm the operation when prompted.

### 7. View Outputs

```bash
terraform output
```

This displays the outputs defined by the Terraform configuration.

### 8. Clean Up Resources

When the resources are no longer needed:

```bash
terraform destroy
```

Review the proposed deletions carefully before confirming. Destroying resources can cause data loss, and some AWS resources may incur charges while they exist.

## 🔑 Important Terraform Commands

| Command | Purpose |
|---|---|
| `terraform init` | Initialize the project |
| `terraform fmt` | Format configuration files |
| `terraform validate` | Validate configuration syntax |
| `terraform plan` | Preview infrastructure changes |
| `terraform apply` | Apply infrastructure changes |
| `terraform output` | Display configured outputs |
| `terraform state list` | List resources in the state |
| `terraform destroy` | Remove managed infrastructure |

## 🔒 Security Best Practices

- Use IAM identities with least-privilege permissions.
- Never upload AWS credentials or sensitive `.tfvars` files.
- Add sensitive files and local state files to `.gitignore`.
- Protect Terraform state because it may contain sensitive information.
- Review every execution plan before applying changes.
- Monitor AWS usage and delete unused resources to control costs.

## 📚 Learning Outcomes

Through this project, I aim to strengthen my understanding of:

- Infrastructure as Code principles.
- AWS resource provisioning and management.
- Terraform configuration and state management.
- Infrastructure automation and reproducibility.
- Cloud security and resource cost management.
- Practical workflows used in DevOps engineering.

## 🎯 Future Enhancements

- Create reusable Terraform modules.
- Provision EC2 instances, security groups, and networking resources.
- Explore remote state storage using Amazon S3.
- Learn environment management and infrastructure reuse.
- Integrate Terraform into CI/CD workflows.
- Explore automated infrastructure provisioning as part of a larger DevOps pipeline.

## 👩‍💻 Author

**Anukriti Gupta**

- GitHub: [@anukritigupta07](https://github.com/anukritigupta07)
- LinkedIn: [Connect with me](https://www.linkedin.com/in/anukritigupta03)
- Portfolio: [Visit my portfolio](https://anukritigupta-portfolio.vercel.app/)

---

⭐ If you find this repository useful, feel free to explore the code and follow my journey into DevOps and cloud engineering.

*Learning by building, automating, and improving — one infrastructure deployment at a time.*

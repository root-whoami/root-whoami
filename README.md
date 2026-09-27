<div align="center">

# ☁️ Hi, I'm root-whoami

<a href="https://github.com/root-whoami">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=38BDF8&center=true&vCenter=true&width=620&lines=echo+%22Welcome+to+my+DevOps+Portfolio%22;Aspiring+DevOps+%26+Cloud+Engineer;Linux+%7C+Python+%7C+Bash+%7C+AWS;Automating+Infrastructure+%26+Workflows" alt="Typing SVG" />
</a>

<p align="center">
  <b>Computer Science Graduate</b> focused on <b>Linux system administration</b>, <b>Python scripting</b>, <b>Bash automation</b>, and building hands-on <b>AWS cloud infrastructure</b>.
</p>

<p align="center">
  <a href="#-about-me">About Me</a> •
  <a href="#-devops-core-principles">Principles</a> •
  <a href="#-technical-skills">Skills</a> •
  <a href="#-featured-project">Featured Project</a> •
  <a href="#-hands-on-roadmap">Roadmap</a> •
  <a href="#-connect">Connect</a>
</p>

</div>

---

## 🖥️ Terminal Overview

```bash
root@cloud-box:~$ cat /etc/whoami.json
{
  "handle": "root-whoami",
  "role": "Aspiring DevOps Engineer",
  "status": "Actively seeking entry-level DevOps / Cloud roles",
  "primary_languages": ["Python", "Bash"],
  "core_focus": ["Linux Administration", "AWS Automation", "Cloud Security"],
  "currently_exploring": ["Docker", "Kubernetes", "Terraform IaC"],
  "current_learning_pace": "1–2 hours / week of disciplined lab building"
}
```

---

## 📌 About Me

* 🎯 **Career Target:** Entry-level DevOps Engineer / Cloud Operations Associate.
* 🐧 **Systems Foundation:** Solid comfort working directly in the Linux terminal, writing automated Bash scripts, and managing system processes.
* 🐍 **Automation Focus:** Using Python and Bash to replace repetitive manual administration with reliable scripts.
* ☁️ **Cloud Focus:** Designing secure, reproducible environments on **AWS** with least-privilege IAM policies.
* 🚀 **Engineering Mindset:** Prioritizing deep understanding and working labs over superficial tool collecting.

---

## 🛡️ DevOps Core Principles

| Principle | How I Apply It |
| :--- | :--- |
| **Least Privilege First** | Never grant wildcard permissions (`*`). Craft granular IAM policies scoped strictly to required operations. |
| **Idempotency** | Ensure every automation script can run repeatedly without throwing duplicate errors or creating orphan cloud resources. |
| **Security Hygiene** | Zero credentials in repositories (`chmod 600`, strict `.gitignore` rules, environment variable injection). |
| **Declarative Infrastructure** | Progressively moving from shell scripts to containerized services and Terraform-managed IaC. |

---

## 💻 Technical Skills

<div align="center">

### Core Systems & DevOps
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)

### Languages & Scripting
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)

### Web & Foundation
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

</div>

---

## 🚀 Active Learning & In-Progress Technologies

I am actively building hands-on competency in the following modern DevOps tools:

| Technology | Specific Focus Areas | Current Progress |
| :--- | :--- | :---: |
| **AWS** | IAM, VPC Subnets, Routing, Security Groups, EC2 | ![In Progress](https://img.shields.io/badge/Status-Hands--on_Labs-blue?style=flat-square) |
| **Docker** | Writing lean multi-stage `Dockerfile`s, Compose orchestration | ![In Progress](https://img.shields.io/badge/Status-In_Progress-yellow?style=flat-square) |
| **Kubernetes** | Pods, Deployments, ClusterIP/NodePort Services, ConfigMaps | ![Learning](https://img.shields.io/badge/Status-Learning-orange?style=flat-square) |
| **Terraform** | HCL syntax, AWS Provider, State Management, Reusable Modules | ![Learning](https://img.shields.io/badge/Status-Learning-orange?style=flat-square) |

---

## ⭐ Featured Flagship Project

### 🔐 [aws-iam-user-automation](https://github.com/root-whoami/aws-iam-user-automation)
> **Automated AWS IAM User Provisioning & Credential Security**

A production-style Bash automation script leveraging the AWS CLI v2 to batch-provision IAM users, enforce mandatory first-login password rotation, attach users to target groups, and protect temporary credentials locally.

```text
  [ Terminal Execution Flow ]
  ├── 1. check_prerequisites() ──> Validates AWS CLI, OpenSSL, and STS Caller Identity
  ├── 2. ensure_group_exists() ──> Idempotently verifies or creates 'Developers' group
  ├── 3. get_usernames()       ──> Validates input format (alphanumeric + symbols, uniqueness)
  ├── 4. process_user()        ──> Checks existing users, provisions new accounts
  ├── 5. generate_password()   ──> OpenSSL cryptographically random passwords
  └── 6. Output & Hygiene      ──> users_passwords.txt locked with chmod 600
```

* **Tech Stack:** Bash (POSIX utils), AWS CLI v2, AWS IAM & STS, OpenSSL.
* **Key Practices:** Idempotent checks, input regex sanitization, `--password-reset-required` policy, POSIX `chmod 600` output, and comprehensive `.gitignore` protection.
* 🔗 **Explore Repository:** [https://github.com/root-whoami/aws-iam-user-automation](https://github.com/root-whoami/aws-iam-user-automation)

---

## 🗺️ Hands-on DevOps Project Roadmap

A project progression designed to demonstrate end-to-end cloud and systems capability:

| Step | Repository / Lab | Primary Competencies | Status |
| :---: | :--- | :--- | :---: |
| **01** | [**`aws-iam-user-automation`**](https://github.com/root-whoami/aws-iam-user-automation) | AWS IAM API, Bash automation, OpenSSL, input validation | ![Completed](https://img.shields.io/badge/Status-Completed-success?style=flat-square) |
| **02** | `linux-server-admin-labs` | User permissions, systemd unit files, process & SSH hardening | ![Next](https://img.shields.io/badge/Status-Up_Next-blue?style=flat-square) |
| **03** | `aws-vpc-infrastructure-lab` | Multi-AZ VPC, Public/Private subnets, IGW, NAT & Route tables | ![Planned](https://img.shields.io/badge/Status-Planned-lightgrey?style=flat-square) |
| **04** | `dockerized-web-app` | Multi-stage Docker builds, non-root execution, Docker Compose | ![Planned](https://img.shields.io/badge/Status-Planned-lightgrey?style=flat-square) |
| **05** | `terraform-aws-infrastructure` | IaC, S3 remote state locking, modular AWS resources | ![Planned](https://img.shields.io/badge/Status-Planned-lightgrey?style=flat-square) |
| **06** | `ci-cd-pipeline-lab` | GitHub Actions automated linting, test runners, AWS deployment | ![Planned](https://img.shields.io/badge/Status-Planned-lightgrey?style=flat-square) |
| **07** | `kubernetes-deployment-lab` | Declarative YAML, Deployments, Services, ConfigMaps & Secrets | ![Planned](https://img.shields.io/badge/Status-Planned-lightgrey?style=flat-square) |

---

## 📊 GitHub Metrics & Activity

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=root-whoami&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="root-whoami GitHub Stats" width="48%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=root-whoami&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" width="48%" />
</div>

<p align="center">
  <sub><i>Note: Language statistics reflect repository code composition across public GitHub repositories, not personal proficiency.</i></sub>
</p>

---

## 📬 Connect With Me

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-root--whoami-181717?style=for-the-badge&logo=github)](https://github.com/root-whoami)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin)](https://github.com/root-whoami)
[![Email](https://img.shields.io/badge/Email-Contact_Me-D14836?style=for-the-badge&logo=gmail&logoColor=white)](https://github.com/root-whoami)

*(Placeholders: LinkedIn and Email will be linked directly to your verified contact channels upon update)*

</div>

---

<div align="center">
  <sub>Built with disciplined engineering standards, continuous learning, and clean documentation.</sub>
</div>

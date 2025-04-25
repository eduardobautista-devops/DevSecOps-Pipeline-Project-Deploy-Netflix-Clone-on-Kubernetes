# DevSecOps Project: Netflix Clone Deployment on Kubernetes

Welcome to my DevSecOps project! This repository showcases a Netflix Clone application deployed as a Docker container on a Kubernetes cluster using a secure, end-to-end CI/CD pipeline using Jenkins. The pipeline integrates several DevOps tools, including:

- **Docker** – Containerization  
- **SonarQube** – Code quality and security analysis  
- **Trivy** – Container vulnerability scanning  
- **Prometheus & Grafana** – Monitoring and observability  
- **ArgoCD** – GitOps continuous delivery tool for Kubernetes 
- **Helm** – Package manager for Kubernetes

---

## 🎬 Inspiration

This project was originally inspired by the YouTube tutorial: https://www.youtube.com/watch?v=g8X5AoqCJHc

However, I’ve made several key improvements and modifications to enhance functionality, security, and automation:

---

## 🔧 Key Improvements

### 🐞 Bug Fixes
- The original `.gitignore` mistakenly excluded `yarn.lock`, which caused the Docker build to fail.
- I resolved this by including the `yarn.lock` file in version control, ensuring consistent dependency resolution across builds.

### 🔐 Security Enhancements
- The tutorial used `--build-arg` to pass the `TMDB_V3_API_KEY` during the Docker build, exposing the key in logs.
- In my pipeline, secrets like `TMDB_V3_API_KEY` are securely injected and never logged or exposed.

### 📚 Documentation Improvements
- I reorganized and enhanced the documentation for clarity, structure, and completeness.
- Missing steps were added and explanations were refined to help others easily reproduce the project.

---

## 🚀 Current Status

- ✅ Manual infrastructure setup and deployment completed successfully.  
> 📄 For detailed **steps and processes**, refer to this [PDF guide](./assets/DevSecOps_Pipeline_Project_Deploy_Netflix_Clone_using_Jenkins_on_Kubernetes.pdf).

- 🔄 Automating provisioning using Infrastructure as Code provisioning to:
  - Save time during setup
  - Reduce manual errors
  - Ensure consistency across environments

---
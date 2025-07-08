---

**“So this was a complete CI/CD project for a Myntra clone application. I started with the NodeJS code hosted on GitHub. Jenkins handles the pipeline — it pulls the code, runs a SonarQube scan to check for bugs and vulnerabilities, and waits for the quality gate to pass.”**

---
**“The tech stack I used includes NodeJS for the app, Jenkins for CI, SonarQube for code quality, Docker for containerization, DockerHub as the registry, ArgoCD for CD using GitOps, EKS for Kubernetes hosting, and Prometheus + Grafana for monitoring.”**

**“Once that’s done, Jenkins builds a Docker image and pushes it to DockerHub. Then instead of deploying directly, I follow a GitOps model — Jenkins updates the Kubernetes deployment file in GitHub with the new image tag.”**

---

**“ArgoCD watches that Git repo. As soon as it detects the change in the manifest, it syncs and deploys the updated app to the Kubernetes cluster running on AWS EKS. This keeps everything version-controlled and automatic.”**

---

**“For security, I enabled HTTPS on ArgoCD using Ingress and cert-manager, and integrated GitHub SSO to avoid using static admin credentials. I also used Trivy to scan Docker images.”**

---

**“For monitoring, I set up Prometheus to collect metrics from the EKS cluster and used Grafana to visualize everything like CPU, memory, and pod health.”**

---

**“So overall, the project showcases how I can build and manage a secure, automated, and observable CI/CD pipeline using modern DevOps tools and best practices.”**



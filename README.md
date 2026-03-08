🚀 Application Deployment using DevOps
📌 Project Overview

This project demonstrates a complete DevOps application deployment pipeline. The objective is to containerize a web application, automate the build process, and deploy it using modern DevOps tools and cloud infrastructure. The project highlights automation, scalability, and efficient application delivery.

🧰 Technologies Used

Docker

Jenkins

Kubernetes (EKS)

Terraform

AWS EC2

GitHub

Linux

Node.js

📂 Project Structure
Project-Application-Deployment
│
├── Dockerfile
├── Jenkinsfile
├── deployment.yaml
├── service.yaml
├── main.tf
├── README.md
└── Screenshots
⚙️ Project Workflow
1️⃣ Clone the Repository
git clone https://github.com/your-repository-link.git
cd repository-name
2️⃣ Build Docker Image
docker build -t application-image .
3️⃣ Run Docker Container
docker run -d -p 3000:3000 application-image
4️⃣ Push Image to Docker Hub
docker tag application-image username/application-image
docker push username/application-image
5️⃣ Infrastructure Setup using Terraform

Terraform is used to provision cloud infrastructure such as EC2 instances and networking components.

terraform init
terraform plan
terraform apply
6️⃣ CI/CD Pipeline using Jenkins

Jenkins automates the following steps:

Pull code from GitHub

Build Docker image

Push image to Docker Hub

Deploy application to Kubernetes cluster

7️⃣ Kubernetes Deployment

Deploy the containerized application to the Kubernetes cluster.

kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

Check running pods:

kubectl get pods
🌐 Application Access

After deployment, the application will be accessible through the Kubernetes service endpoint.

Example:

http://<load-balancer-ip>:3000
📸 Project Screenshots

Screenshots of the deployment process are available in the Screenshots folder.

Examples include:

Docker build

Jenkins pipeline

Kubernetes pods

Application running in browser

🔐 Security Best Practices

Sensitive data should not be pushed to GitHub

Use .gitignore to exclude secret files

Use environment variables for credentials

🎯 Learning Outcomes

Understanding CI/CD pipeline

Containerizing applications with Docker

Infrastructure as Code using Terraform

Deploying applications using Kubernetes

Automating workflows with Jenkins

👨‍💻 Author

Darwin Prem Kumar R

DevOps Engineer | Cloud & Automation Enthusiast


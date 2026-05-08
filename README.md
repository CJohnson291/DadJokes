# DadJokes
Dad Jokes API — Azure Container Apps | Cosmos DB | Docker | Terraform

A fully containerised Node.js Dad Jokes API deployed on Azure using:
• Azure Container Apps (serverless containers)
• Azure Cosmos DB (NoSQL) for joke storage
• Azure Container Registry (ACR) for image hosting
• Docker for building and packaging the API
• Terraform for Infrastructure‑as‑Code
The API exposes JSON and HTML-rendered joke endpoints and is fully cloud‑native, reproducible, and deployed end‑to‑end using IaC + containers.

📌 Features
• Node.js Express API
• Cosmos DB NoSQL backend
• Clean JSON responses
• HTML-rendered joke pages
• Dockerised application
• Image pushed to ACR
• Deployed to Azure Container Apps
• Terraform-managed infrastructure

GET /joke/:id returns JSON format (see screenshots)

GET /joke/:id/html Returns the same joke rendered as a simple HTML page (see screenshots)

🧱 Architecture Overview
• Cosmos DB stores jokes in a container partitioned by /id
• Node.js Express API reads jokes from Cosmos DB
• Docker packages the API into a container image
• ACR stores the image
• Azure Container Apps runs the container in a serverless environment
• Terraform provisions:
	◦ Resource group
	◦ Cosmos DB account, DB, container
	◦ ACR
	◦ Container App environment
	◦ Container App
This architecture mirrors real-world cloud-native deployments.

🎯 Why This Project Matters
This project demonstrates:
• Cloud-native deployment
• Infrastructure as Code
• Containerisation
• Azure PaaS services
• Real-world architecture patterns
• Clean API design
• Ability to troubleshoot and deliver a working cloud system end-to-end

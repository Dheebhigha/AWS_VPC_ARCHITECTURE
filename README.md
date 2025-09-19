# Secure VPC Architecture with Public and Private Subnets  

## 📌 Project Overview  
This project demonstrates the design and deployment of a **secure, production-grade Virtual Private Cloud (VPC) architecture** on AWS.  
The architecture is carefully structured to balance **security, scalability, and reliability**.  

- The setup spans **two Availability Zones (AZs)** to ensure high availability and fault tolerance.  
- Both **public and private subnets** are provisioned in each AZ, providing logical separation of resources.  

---

## 🌐 Public Subnets  
- Each public subnet contains a **NAT Gateway** that allows outbound internet access for private resources, while preventing inbound exposure.  
- A **Load Balancer** is deployed to manage and distribute incoming traffic across multiple backend servers, ensuring seamless performance under varying workloads.  

---

## 🔒 Private Subnets  
- Application **servers reside in private subnets**, fully shielded from direct internet access.  
- These servers are managed by an **Auto Scaling Group**, which automates deployment, scaling, and termination based on workload demand.  
- This ensures the environment remains **cost-efficient** while being highly responsive to traffic changes.  
- Servers can securely communicate with the internet through the **NAT Gateway**, only when necessary.  

---

## ⚡ Key Features  
- **Reliability:** Resources are distributed across multiple AZs for fault tolerance.  
- **Scalability:** Auto Scaling adapts dynamically to workload fluctuations.  
- **Security:** Private subnets, security groups, and NAT gateways safeguard sensitive resources.  
- **Efficiency:** Load balancing optimizes traffic handling and ensures a smooth user experience.  

---

## 📄 Documentation  
All detailed explanations of the architecture, design choices, and flow are consolidated into a **comprehensive PDF report**.  
The PDF is attached within this repository and serves as the **complete project documentation** for reference and review.  

---


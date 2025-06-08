# 🌍 Study Abroad Safety System – Serverless Application on AWS

## 🌟 Project Overview

This project presents a fully cloud-native Study Abroad System built to enhance student safety and communication during international travel. Designed with a serverless-first architecture, the application supports three main user roles—students, faculty, and administrators—and provides real-time check-ins, automated alerts, and secure oversight of travel programs.

The system was developed as part of an academic capstone at Texas A&M University and simulates real-world challenges in cloud infrastructure, event-driven logic, role-based access, and automated deployment.

---

## 👤 User Roles

- **Students**: Check in during travel, update locations, and trigger emergency alerts  
- **Faculty**: Monitor students, respond to emergencies, and create custom check-in statuses  
- **Administrators**: Manage system-wide access, class/trip configurations, and user assignments

---

## 🔑 Key Features

- Geolocation-based student tracking  
- Scheduled and on-demand check-ins  
- Emergency alert system with faculty notification  
- Role-based access control (RBAC) via Amazon Cognito  
- Serverless infrastructure with automated CI/CD  
- Fully modular Infrastructure as Code using Terraform

---

## 🏗️ Architecture Overview

The system uses a scalable, event-driven architecture powered by AWS. Key components include:

- **Frontend**: HTML, CSS, JavaScript hosted on **Amazon S3** and served through **CloudFront**  
- **Backend**: Stateless **AWS Lambda** functions invoked via **Amazon API Gateway**  
- **Database**: **Amazon DynamoDB** tables for Users, Locations, and ClassTrips  
- **Authentication**: **Amazon Cognito** User Pools with RBAC  
- **Notifications**: Real-time alerts via **Amazon SNS**  
- **Infrastructure as Code**: **Terraform** for provisioning and environment management  
- **CI/CD**: **GitHub Actions** for full-stack deployments and cache invalidation

---

## 📂 Project Structure

<img width="629" alt="image" src="https://github.com/user-attachments/assets/34e47eb9-42db-40ff-96f6-7d95ac2ba7d8" />




---

## 🚀 Getting Started

### ✅ Prerequisites
- AWS account with IAM permissions and access keys
- Terraform CLI v1.6+
- Configured GitHub Secrets:
  - `AWS_ACCESS_KEY_ID`
  - `AWS_SECRET_ACCESS_KEY`
  - `AWS_S3_BUCKET`
  - `CLOUDFRONT_DISTRIBUTION_ID`

### ⚙️ Deployment Steps
1. Navigate to the GitHub repository
2. Open the **Actions** tab
3. Trigger the **Full Deploy Pipeline**
4. For manual setup, refer to [Admin Deployment Guide](./docs/admin_deployment.md)

---

## 🧑‍💻 System Usage

### 🎒 Student Dashboard
- Share current location
- Select check-in status (e.g., "At Hotel", "Exploring City")
- Submit comments or emergency alerts

### 👩‍🏫 Faculty Dashboard
- Track student location history
- Send check-in requests
- Customize status labels
- Review SOS alerts

### 🛠️ Admin Dashboard
- Configure new trips/classes
- Assign students and faculty
- Monitor global system activity

---

## 📘 Documentation

- [Student Guide](./public/README.md#student-dashboard)  
- [Faculty Guide](./public/README.md#faculty-dashboard)  
- [Admin Guide](./public/README.md#admin-dashboard)  
- [Backend Functions](./backend/README.md)  
- [Terraform & Infrastructure](./terraform-project/README.md)

---

## 🧰 Technologies Used

| Layer             | Tools & Services                          |
|------------------|-------------------------------------------|
| Frontend         | HTML5, CSS3, JavaScript (ES6)             |
| Backend          | AWS Lambda (Python/Node.js), API Gateway |
| Data Storage     | Amazon DynamoDB                           |
| Authentication   | Amazon Cognito                            |
| Notifications    | Amazon SNS                                |
| Hosting/CDN      | Amazon S3 + CloudFront                    |
| Infrastructure   | Terraform                                 |
| CI/CD            | GitHub Actions                            |

---

## 🤝 Contributing

1. Fork this repo  
2. Create a feature branch (`git checkout -b feature/your-feature`)  
3. Commit your changes (`git commit -m "Add: feature description"`)  
4. Push and open a Pull Request  

---

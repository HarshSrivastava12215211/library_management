LIBRARY MANAGEMENT SYSTEM

This project is a simple Library Management System built using HTML, CSS, JavaScript, Flask, and SQLite. It allows users to add, view, and manage books in a digital library. The project is fully containerized using Docker and follows a CI/CD pipeline implemented via Jenkins with GitHub Webhooks for automated testing and deployment.

Features
Add and view book records

Search for books by name or author

Update or delete book entries

Clean and responsive UI

SQLite for lightweight database management

Fully Dockerized environment

CI/CD pipeline using Jenkins

Automated testing and deployment triggered by GitHub Webhooks

Technologies Used
Frontend: HTML, CSS, JavaScript

Backend: Python (Flask)

Database: SQLite

Containerization: Docker

CI/CD: Jenkins

Version Control: Git & GitHub

Image Hosting: DockerHub

 Setup Instructions
Local Setup
Clone the Repository

bash
Copy
Edit
git clone https://github.com/HarshSrivastava12215211/library-management-app.git
cd library-management-app
Run Locally (Without Docker)

bash
Copy
Edit
pip install -r requirements.txt
python app.py
Visit http://localhost:5000

🐳 Docker Setup
Build Docker Image

bash
Copy
Edit
docker build -t your-dockerhub-username/library-app .
Run Docker Container

bash
Copy
Edit
docker run -d -p 5000:5000 your-dockerhub-username/library-app
Push to DockerHub

bash
Copy
Edit
docker login
docker push your-dockerhub-username/library-app
CI/CD Pipeline (Jenkins + Webhooks)
Jenkins Pipeline Steps
Clone Code from GitHub

Build Docker Image

Run Automated Tests

Push Image to DockerHub

Deploy Container

GitHub Webhook Setup
Go to your GitHub repo → Settings → Webhooks

Add your Jenkins webhook URL:
http://<your-jenkins-server>/github-webhook/

Content type: application/json

Trigger on: push events

Automated Testing
Write and place test scripts (e.g., test_app.py) in the project.

Jenkins runs these tests on each push using pytest or similar framework.

📂 Project Structure
cpp
Copy
Edit
├── app.py
├── templates/
│   └── index.html
├── static/
│   ├── style.css
│   └── script.js
├── Dockerfile
├── requirements.txt
├── test_app.py
└── README.md
📸 Screenshots

![image](https://github.com/user-attachments/assets/a061524b-4b76-475b-9676-5f6c0ee6f881)


📦 DockerHub
Image: docker.io/your-dockerhub-username/library-app

🙌 Acknowledgements
Flask Documentation

Docker Docs

Jenkins Community

GitHub Webhooks

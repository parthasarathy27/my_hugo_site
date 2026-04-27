# 🚀 Hugo Website Deployment with Cloud Build & Firebase

This project demonstrates a complete CI/CD pipeline for deploying a static website built with Hugo using Google Cloud Build and Firebase Hosting.

## 📌 Overview

This repository contains a Hugo-based static website that is automatically built and deployed using a Cloud Build pipeline whenever changes are pushed to the main branch.

The deployment process includes:
- Building the static site using Hugo
- Deploying the site to Firebase Hosting
- Automating the workflow with Google Cloud Build triggers

## 🛠️ Tech Stack

- **Hugo** – Static Site Generator
- **Firebase Hosting** – CDN-based hosting with SSL
- **Google Cloud Build** – CI/CD pipeline automation
- **GitHub** – Version control & trigger source

## ⚙️ Project Architecture


GitHub Repo → Cloud Build Trigger → Build Process → Firebase Hosting


## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/my_hugo_site.git
cd my_hugo_site
2. Install Hugo
/tmp/installhugo.sh
3. Run Locally
/tmp/hugo server -D --bind 0.0.0.0 --port 8080

Visit:

http://localhost:8080
🔥 Deployment (Manual)
/tmp/hugo
firebase deploy
🤖 CI/CD Pipeline (Cloud Build)

The pipeline is configured using cloudbuild.yaml.

Pipeline Steps:
Download Hugo & Firebase CLI
Build static site using Hugo
Deploy to Firebase Hosting
Trigger:
Triggered on push to main branch
📂 Important Files
cloudbuild.yaml → CI/CD pipeline config
config.toml → Hugo configuration
themes/ → Website theme
content/ → Site content
🌐 Live Site

Firebase Hosting URL will be generated after deployment.

🧪 Testing Pipeline
git add .
git commit -m "Update site"
git push origin main

This will automatically trigger deployment.

🔐 Notes
Firebase provides SSL by default
Cloud Build runs in a serverless environment
No backend server required (fully static site)
📚 Learning Outcomes
Static site deployment
CI/CD pipeline creation
GitHub integration with Cloud Build
Firebase Hosting usage
🏁 Conclusion

This project showcases how to automate website deployment using modern DevOps practices on Google Cloud.

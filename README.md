# Hello Java Maven (Jenkins Freestyle Build)

A minimal Java “Hello World” project built with **Maven** and compiled by **Jenkins** to demonstrate a basic CI build.

---

## 🌟 Project Goal
- Build a simple Java app with Maven (`clean package`)
- Run the JAR output locally
- Show Jenkins Freestyle job configuration and a successful build

---

## 🧰 Tech & Tools
- **Java JDK** (8/11/21 all fine)
- **Maven** (3.x)
- **Jenkins** (Freestyle job)
- **Git** (optional if you run locally only)

---

## 📁 Repository Structure

hello-java-maven/
├─ pom.xml
└─ src/
└─ main/
└─ java/
└─ HelloWorld.java

🏗️ Build with Jenkins (Freestyle)

Open: http://localhost:8080

Configure Tools

Manage Jenkins → Global Tool Configuration

JDK: Add your JDK (e.g., C:\Program Files\Java\jdk-21)

Maven: Add Maven

Create Job

New Item → Freestyle project (name: hello-java-maven)

Source Code Management → Git

Repo URL: https://github.com/jaspreet237/hello-java-maven.git

Branch: */main

Build → Add build step → Invoke top-level Maven targets

Maven Version: 3.9.11

Goals: clean package

Save → Build Now

Verify

Console Output should end with: BUILD SUCCESS

Artifact path: target/hello-1.0.jar

Run the built app

From the Jenkins workspace (Windows example):

java -cp C:\ProgramData\Jenkins\.jenkins\workspace\hello-java-maven\target\hello-1.0.jar HelloWorld


🧯 Quick Troubleshooting

JAVA_HOME not set
Configure JDK under Global Tool Configuration and select it in the job.

## 🌟 ScreenShots
<img width="910" height="401" alt="image" src="https://github.com/user-attachments/assets/c0c571da-2c3f-4ff5-a6f0-bf7020413d6e" />

<img width="1335" height="579" alt="image" src="https://github.com/user-attachments/assets/dca6e6c6-8f6f-402f-917a-0ddfcd3568a5" />

<img width="1025" height="57" alt="image" src="https://github.com/user-attachments/assets/bbba0838-62cb-4243-bab9-e2ed576ed7a3" />

<img width="673" height="192" alt="image" src="https://github.com/user-attachments/assets/7e25c6f7-6602-45d1-b4b0-c2db9b014ed9" />




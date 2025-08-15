
# Java Maven Web App - Jenkins CI/CD Deployment

## 📌 Project Overview
This is a simple **Java Maven Hello World Web Application** that is deployed on **Apache Tomcat** using a Jenkins CI/CD pipeline.

## 🚀 Workflow
1. Developed a simple `Hello World` web application using Maven.
2. Pushed source code to a GitHub repository.
3. Configured Jenkins to pull the latest code from GitHub.
4. Jenkins builds the project using Maven (`mvn clean package`).
5. Generated WAR file is automatically deployed to Tomcat.
6. Verified deployment by accessing the web application in the browser.

## 🛠️ Tech Stack
- **Java**
- **Maven**
- **Apache Tomcat**
- **Jenkins**
- **Git & GitHub**
- **Docker** (if used for Jenkins/Tomcat)

## ⚙️ How to Build and Run Locally
```bash
# Clone repository
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>

# Build with Maven
mvn clean package

# Deploy WAR file to Tomcat webapps/ directory
cp target/*.war $TOMCAT_HOME/webapps/



# Maven Commands
mvn -v	                -->    Check Maven version and installation.
mvn clean	              -->    Removes the target/ directory (compiled code, build artifacts).
mvn compile	            -->     Compiles the source code in src/main/java.
mvn test	              -->    Runs unit tests in src/test/java.
mvn package	            -->    Compiles code, runs tests, and packages into a JAR/WAR (based on pom.xml).



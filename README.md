# DevOps Task 1: Automate Code Deployment Using CI/CD Pipeline

## 🚀 Objective
Set up an automated CI/CD pipeline using GitHub Actions to build a Node.js web application, containerize it using Docker, and push the final image to Docker Hub.

## 🛠️ Tools Used
* **GitHub & GitHub Actions:** For version control and automated workflow execution.
* **Node.js:** For running the sample backend web application.
* **Docker & Docker Hub:** For containerizing the application and storing the deployment image.

## ⚙️ How the Pipeline Works
1. **Trigger:** The workflow is triggered automatically on every `git push` to the `main` branch.
2. **Checkout & Setup:** The GitHub Actions runner checks out the repository code and sets up the Node.js environment.
3. **Docker Login:** Authenticates with Docker Hub securely using encrypted repository secrets (`DOCKER_USERNAME` and `DOCKER_PASSWORD`).
4. **Build & Push:** Builds the Docker container from the `Dockerfile` and pushes the updated image to Docker Hub.

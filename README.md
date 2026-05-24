# Jenkins CI/CD Pipeline Project

This repository demonstrates a basic Continuous Integration and Continuous Deployment (CI/CD) workflow using **Jenkins**, **Docker**, and **C++**. It automates the process of compiling C++ source files and packaging the application within a Docker container.

## 🚀 Repository Structure

* **`Dockerfile`**: Defines the environment and steps needed to build the Docker image for the application.
* **`Jenkinsfile`**: Contains the pipeline script (automation steps) that Jenkins executes to build and test the project.
* **`main/`**: Directory containing the main C++ source code (including `hello.cpp`).
* **`new.cpp`**: Additional C++ source files or experiments.
* **`Makefile`**: (If applicable) Used to simplify the compilation commands for the C++ code.

---

## 🛠️ Prerequisites

To run this project locally or via a CI/CD server, you will need:
* [Docker](https://www.docker.com/) installed and running.
* [Jenkins](https://www.jenkins.io/) installed with the Docker pipeline plugins enabled.
* A C++ compiler (like `g++`) if you wish to compile manually outside of Docker.

---

## 🏗️ How it Works

### 1. Jenkins Pipeline (`Jenkinsfile`)
The repository includes a `Jenkinsfile` that automates your build stages. When a change is pushed to this repository, Jenkins automatically:
1.  **Clones** the repository.
2.  **Compiles** the C++ source files (`hello.cpp`, `new.cpp`).
3.  **Builds** a Docker image using the provided `Dockerfile`.

### 2. Dockerization (`Dockerfile`)
The application is containerized to ensure it runs consistently across any environment. The `Dockerfile` handles installing the necessary build tools, copying the source files, compiling the binary, and defining the execution command.

---

## 💻 Manual Local Setup

If you want to test the Docker setup manually on your machine without running Jenkins:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/dnmeghana/PES2UG20CS519_jenkins.git](https://github.com/dnmeghana/PES2UG20CS519_jenkins.git)
   cd PES2UG20CS519_jenkins
2. **Clone the repository:**
   ```bash
   docker build -t cpp-jenkins-app .
3. **Run the Container:**
   ```bash
   docker build -t cpp-jenkins-app .

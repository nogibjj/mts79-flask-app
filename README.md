[![Build and Push Docker Image](https://github.com/nogibjj/mts79-flask-app/actions/workflows/cicd.yml/badge.svg)](https://github.com/nogibjj/mts79-flask-app/actions/workflows/cicd.yml)
# **My Python Docker App**

This is a simple Python application containerized using Docker. It demonstrates core functionalities of Python applications running in a containerized environment. The project integrates a CI/CD pipeline to build and push the Docker image to Docker Hub.

[Click here to view the Docker image](https://hub.docker.com/r/monasaeed/my_python_app)  

---

## **Features**
- **Containerization**: Application runs in an isolated Docker environment.
- **CI/CD Support**: Builds and deploys the Docker image to Docker Hub.

---

## **Project Structure**
- **`app.py`**: Main Python application file.
- **`Dockerfile`**: Configuration file for building the Docker image.
- **`Makefile`**: Simplifies Docker commands for building, running, and pushing the image.

---

## **Prerequisites**
- Python 3.9+
- Docker
- Make

---

## **Usage**

### **1. Clone the Repository**
```bash
git clone <https://github.com/nogibjj/mts79-flask-app>
cd <mts79-flask-app>
```

### **2. Build the Docker Image**
```bash
make build
```

### **3. Run the Application**
```bash
make run
```
Access the app in your browser at `http://localhost:5000`.

### **4. Push to Docker Hub**
Ensure you are logged into Docker:
```bash
make login
```
Then push the image:
```bash
make push
```

### **5. Clean Up Docker**
To stop and remove containers and images:
```bash
make clean
```

### **6. Show Docker Images and Containers**
To list images:
```bash
docker images
```
To list running containers:
```bash
docker ps
```

---

## **Docker Hub Details**
- **Docker Image Name**: `monasaeed/my_python_app`
- **Tag**: `latest`

---

## **Resources**
- [Docker Documentation](https://docs.docker.com/)
- [Flask Documentation](https://flask.palletsprojects.com/)
- [GitHub Actions](https://docs.github.com/en/actions)
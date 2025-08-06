# 🐳 Docker Crash Course

> Your quick and practical guide to Docker — the tool for building, shipping, and running containers.

*A one-liner guide for each command to help you get productive with Docker fast.*

---

## 📦 Basic Commands

```bash
# Check Docker version
docker --version
# Show system-wide info
docker info
# List running containers
docker ps
# List all containers (including stopped)
docker ps -a
```

---

## 🐋 Images

```bash
# List all local images
docker images
# Download image from Docker Hub
docker pull <image>
# Remove image
docker rmi <image>
```

---

## 🚀 Containers

```bash
# Run container from image
docker run <image>
# Run with custom name and auto-remove after exit
docker run --rm --name <name> <image>
# Run interactively (like a shell)
docker run -it <image> /bin/bash
# Start/stop/restart a container
docker start|stop|restart <container>
# Remove a container
docker rm <container>
```

---

## 🗂️ Volumes & Files

```bash
# Mount a local folder into container
docker run -v $(pwd):/app <image>
# Copy file from container to host
docker cp <container>:/file ./
# Copy file from host to container
docker cp ./file <container>:/file
```

---

## 🏗️ Build & Tag Images

```bash
# Build image from Dockerfile
docker build -t <tag> .
# Tag an existing image
docker tag <image> <username>/<repo>:<tag>
# Push to Docker Hub
docker push <username>/<repo>
```

---

## 🧹 Clean Up

```bash
# Remove all stopped containers
docker container prune
# Remove all unused images
docker image prune -a
# Remove unused volumes
docker volume prune
```

---

## 🔍 Inspect & Logs

```bash
# Inspect container info
docker inspect <container>
# View logs from container
docker logs <container>
# View real-time logs
docker logs -f <container>
```

---

## 🔄 Docker Compose

```bash
# Start all services in background
docker-compose up -d
# Stop all services
docker-compose down
# Build services
docker-compose build
# View logs
docker-compose logs -f
```

---

## ✅ Pro Tips

* Use `.dockerignore` like `.gitignore` to exclude files from build context.
* Always tag your images with versions, not just `latest`.
* Use `docker system df` to check space usage.

---

Happy containerizing! 📦🐳

### **I. Foundations & Core Concepts**

1.  **Introduction to Containerization**
    *   What is a Container? (vs. Virtual Machines)
    *   The Problem Containers Solve
    *   Benefits of Using Containers (Portability, Efficiency, Isolation)

2.  **Understanding Docker**
    *   What is Docker?
    *   Docker Architecture: Client-Server Model
    *   Docker Daemon (`dockerd`)
    *   Docker Client (`docker` CLI)
    *   Docker Desktop (for Windows/Mac)

3.  **Key Docker Objects**
    *   **Images:** Read-only templates with instructions.
    *   **Containers:** Runnable instances of an image.
    *   **Dockerfile:** A text file to build a custom image.

### **II. Working with Docker Images**

1.  **Docker Registries & Repositories**
    *   Docker Hub (Public Registry)
    *   Pulling Public Images (`docker pull`)
    *   Pushing Images to a Registry (`docker push`)
    *   Private Registries (AWS ECR, Google GCR, Azure ACR, self-hosted)

2.  **Image Management**
    *   Listing Images (`docker images`)
    *   Inspecting Images (`docker inspect`)
    *   Removing Images (`docker rmi`)
    *   Understanding Image Layers and Caching

### **III. Working with Docker Containers**

1.  **Container Lifecycle**
    *   Running a Container (`docker run`)
    *   Common `docker run` flags (`-d`, `-p`, `-v`, `--name`, `-it`)
    *   Listing Running & Stopped Containers (`docker ps -a`)
    *   Stopping a Container (`docker stop`)
    *   Starting a Container (`docker start`)
    *   Restarting a Container (`docker restart`)
    *   Removing a Container (`docker rm`)

2.  **Container Interaction**
    *   Running Commands in a Running Container (`docker exec`)
    *   Attaching to a Running Container (`docker attach`)
    *   Viewing Container Logs (`docker logs`)

### **IV. Building Custom Images: The Dockerfile**

1.  **Dockerfile Instructions**
    *   `FROM` (Base Image)
    *   `RUN` (Executing Commands)
    *   `COPY` & `ADD` (Adding Files)
    *   `WORKDIR` (Setting Working Directory)
    *   `EXPOSE` (Documenting Ports)
    *   `ENV` (Setting Environment Variables)
    *   `CMD` (Default Command to Run)
    *   `ENTRYPOINT` (Configuring a Container to Run as an Executable)

2.  **Best Practices for Dockerfiles**
    *   Using `.dockerignore` files
    *   Minimizing Image Size (using small base images, combining `RUN` commands)
    *   Leveraging Layer Caching Effectively
    *   Security Best Practices (not running as root)

### **V. Data Persistence & Management**

1.  **Docker Storage**
    *   The Writeable Container Layer (Ephemeral Storage)
    *   **Docker Volumes:** The preferred mechanism for persisting data.
        *   Creating and Managing Volumes (`docker volume create`)
        *   Using Named and Anonymous Volumes
    *   **Bind Mounts:** Mapping a host directory to a container directory.
    *   **tmpfs Mounts:** Storing data in host memory.

### **VI. Networking**

1.  **Docker Network Drivers**
    *   `bridge`: Default network for standalone containers.
    *   `host`: Removes network isolation between container and host.
    *   `none`: Disables all networking.
    *   `overlay`: Connects multiple Docker daemons (for Swarm).
    *   `macvlan`: Assigns a MAC address to a container.

2.  **Network Management**
    *   Listing Networks (`docker network ls`)
    *   Creating a Custom Network (`docker network create`)
    *   Connecting Containers to Networks
    *   Docker DNS for Container Discovery

### **VII. Docker Compose (Orchestration for Development)**

1.  **Introduction to Docker Compose**
    *   What is Docker Compose?
    *   The `docker-compose.yml` File Structure (YAML)

2.  **Compose File Key Sections**
    *   `services`: Defining your application's components (web, db, cache).
    *   `networks`: Defining custom networks.
    *   `volumes`: Defining named volumes for data persistence.

3.  **Compose Commands**
    *   `docker-compose up` (Start all services)
    *   `docker-compose down` (Stop and remove all services)
    *   `docker-compose ps`, `logs`, `exec`

### **VIII. Advanced Topics**

1.  **Docker Security**
    *   Principle of Least Privilege
    *   Running as Non-Root User
    *   Image Security Scanning
    *   Understanding Linux Capabilities
    *   Security Profiles (AppArmor, SELinux)

2.  **Container Orchestration (Production)**
    *   **Docker Swarm Mode:** Native Docker clustering.
        *   Swarm Architecture (Managers & Workers)
        *   Services, Tasks, and Replicas
        *   Rolling Updates
    *   **Kubernetes (K8s):** The industry standard.
        *   Pods, Deployments, Services
        *   Helm Charts
        *   Ingress Controllers

3.  **CI/CD with Docker**
    *   Building Docker Images in a Pipeline (e.g., Jenkins, GitLab CI, GitHub Actions)
    *   Multi-stage Builds for Creating Lean Production Images
    *   Pushing Images to a Registry from CI

4.  **Image Creation & Optimization**
    *   **Multi-stage Builds:** Separating build-time and run-time dependencies.
    *   **Distroless Images:** Extremely minimal and secure images.

5.  **Docker Internals (Deep Dive)**
    *   **Namespaces** (pid, net, ipc, mnt, uts)
    *   **Control Groups (cgroups)**
    *   **Union File Systems (Overlay2, AUFS)**

### **IX. Ecosystem & Tools**

1.  **Monitoring & Logging**
    *   `docker stats`
    *   `docker logs`
    *   Integrating with Prometheus & Grafana
    *   Centralized Logging with ELK Stack or Loki

2.  **Alternative Runtimes & Standards**
    *   **containerd:** Industry-standard container runtime.
    *   **Podman:** A daemonless alternative to Docker.
    *   **Open Container Initiative (OCI):** Standards for images and runtimes.

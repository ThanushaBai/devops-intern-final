# DevOps Intern Final Assessment

**Name:** Thanusha Bai V  
**Date:** August 2026

## Project Overview

This repository contains my submission for the DevOps Intern Final Assessment.

The project demonstrates fundamental DevOps concepts including:

- Git & GitHub
- Linux Shell Scripting
- Docker Containerization
- GitHub Actions (CI/CD)
- Nomad Job Deployment
- Grafana Loki Monitoring

---

## Project Structure

```
devops-intern-final/
│
├── .github/
│   └── workflows/
│       └── ci.yml
│
├── monitoring/
│   └── loki_setup.txt
│
├── nomad/
│   └── hello.nomad
│
├── scripts/
│   └── sysinfo.sh
│
├── hello.py
├── Dockerfile
└── README.md
```

---

# Step 1 – Git & GitHub

Created a public GitHub repository containing:

- README.md
- hello.py

The Python script prints:

```python
Hello, DevOps!
```

Run:

```bash
python hello.py
```

---

# Step 2 – Linux Shell Script

Created:

```
scripts/sysinfo.sh
```

The script displays:

- Current user
- Current date
- Disk usage

Run:

```bash
bash scripts/sysinfo.sh
```

---

# Step 3 – Docker

Created a Dockerfile to containerize the Python application.

Build the Docker image:

```bash
docker build -t hello-devops .
```

Run the container:

```bash
docker run hello-devops
```

Expected Output:

```
Hello, DevOps!
```

---

# Step 4 – GitHub Actions (CI/CD)

A GitHub Actions workflow automatically runs:

```bash
python hello.py
```

on every push to the repository.

Workflow file:

```
.github/workflows/ci.yml
```

---

# Step 5 – Nomad Deployment

Created a Nomad job file:

```
nomad/hello.nomad
```

Run:

```bash
nomad job run nomad/hello.nomad
```

This deploys the Docker container as a Nomad service using minimal CPU and memory resources.

---

# Step 6 – Grafana Loki Monitoring

Started Loki using Docker:

```bash
docker run -d --name loki -p 3100:3100 grafana/loki:3.0.0
```

Verify Loki is running:

```
http://localhost:3100/ready
```

Logs and setup instructions are available in:

```
monitoring/loki_setup.txt
```

---

# Technologies Used

- Git
- GitHub
- Linux
- Bash
- Docker
- GitHub Actions
- Nomad
- Grafana Loki
- Python

---

# Author

**Thanusha Bai V**

DevOps Intern Final Assessment

August 2026
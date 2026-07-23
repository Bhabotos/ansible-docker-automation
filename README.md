# Docker Installation Automation with Ansible

## Project Overview

This project automates Docker installation and container deployment on Ubuntu using Ansible.

The automation performs the following tasks:

- Update Ubuntu packages
- Install Docker Engine
- Install Docker Compose Plugin
- Enable Docker Service
- Verify Docker Installation
- Deploy Nginx Container
- Deploy Redis Container
- Deploy PostgreSQL Container

---

## Technologies

- Ubuntu 24.04
- Ansible
- Docker
- Docker Compose
- PostgreSQL
- Redis
- Nginx

---

## Project Structure

```text
ansible-docker-automation/
├── ansible.cfg
├── inventory/
├── group_vars/
├── playbooks/
├── roles/
├── docker-compose.yml
└── README.md
```

---

## Run Project

```bash
ansible-playbook playbooks/site.yml
```

---

## Verify

```bash
docker ps
```

---

## Browser

```
http://localhost
```

---

## PostgreSQL

```bash
docker exec -it postgres psql -U admin -d mydb
```

---

## Redis

```bash
docker exec -it redis redis-cli
```

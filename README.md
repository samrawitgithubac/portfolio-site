# Project Setup Guide

This guide will walk you through setting up and running the application (backend + frontend) locally using Docker.

---

## Prerequisites
Before starting, make sure you have the following installed:
- [Git](https://git-scm.com/)
- [Docker](https://www.docker.com/) & [Docker Compose](https://docs.docker.com/compose/)

---

## 1. Clone the Repository
```bash
git clone https://github.com/Zekariyas-Teshager/NaturalContraceptionMethod.git
cd NaturalContraceptionMethod
```

---

## 2. Environment Variables

1. Download the `.env` file from **Telegram**.
2. Paste the `.env` file into the **backend** directory.

---

## 3. Build and Run the Application

From the root project directory, run:

```bash
docker compose build
docker compose up
```

This will:

* Build the backend and frontend services.
* Start all required containers (API server, database, etc.).

---

## 4. Access the Application

Once the containers are up and running:

* **Swagger API Documentation:** [http://localhost:3000/api-docs#/](http://localhost:3000/api-docs#/)
* **Backend Base URL:** [http://localhost:3000/](http://localhost:3000/)

---

## 5. Stopping the Application

To stop all running containers:

```bash
docker compose down
```

---

## Notes

* If you make changes to the backend code, you may need to rebuild:

```bash
docker compose build backend
docker compose up
```

* If you encounter port conflicts, update the ports in `docker-compose.yml`.

---

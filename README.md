# 🚀 ELT Data Pipeline Project (Docker + PostgreSQL)

## 📌 Overview

This project demonstrates an **ELT (Extract → Load → Transform)** data pipeline built using **Docker containers** and **PostgreSQL databases**.
The pipeline extracts data from a source database, loads it into a destination database, and performs transformations inside the data warehouse.

This project is designed to help understand **modern data engineering workflows** and container-based data pipelines.

---

## 🏗️ Architecture

```
Source PostgreSQL  ──►  ELT Script  ──►  Destination PostgreSQL
        (Extract)          (Load)            (Transform)
```

### Components

* **Source Database** – Raw data storage
* **Destination Database** – Data warehouse
* **Docker Compose** – Container orchestration
* **ELT Script** – Handles extraction, loading, and transformation

---

## ⚙️ Tech Stack

* Docker & Docker Compose
* PostgreSQL
* Python (ELT scripting)
* SQL
* WSL (Windows Subsystem for Linux)
* VS Code

---

## 📂 Project Structure

```
elt/
│
├── docker-compose.yml
├── elt_script.py
├── requirements.txt
├── .env
└── README.md
```

---

## ▶️ Getting Started

### 1️⃣ Clone Repository

```bash
git clone https://github.com/<your-username>/elt-project.git
cd elt-project
```

### 2️⃣ Start Containers

```bash
docker compose up -d
```

### 3️⃣ Check Running Containers

```bash
docker ps
```

### 4️⃣ Access PostgreSQL Container

```bash
docker exec -it elt-destination_postgres-1 psql -U postgres
```

---

## 🔄 ELT Workflow

1. **Extract**
   Data is read from the source PostgreSQL database.

2. **Load**
   Extracted data is loaded into the destination database.

3. **Transform**
   SQL transformations clean and structure the data for analytics.

---

## 🧪 Useful Commands

Start services:

```bash
docker compose up -d
```

Stop services:

```bash
docker compose down
```

View logs:

```bash
docker compose logs
```

---

## 🔐 Environment Variables

Sensitive configuration is stored in `.env` file.
# 🚀 ELT Data Pipeline Project (Docker + PostgreSQL)

## 📌 Overview

This project demonstrates an **ELT (Extract → Load → Transform)** data pipeline built using **Docker containers** and **PostgreSQL databases**.
The pipeline extracts data from a source database, loads it into a destination database, and performs transformations inside the data warehouse.

This project is designed to help understand **modern data engineering workflows** and container-based data pipelines.

---

## 🏗️ Architecture

```
Source PostgreSQL  ──►  ELT Script  ──►  Destination PostgreSQL
        (Extract)          (Load)            (Transform)
```

### Components

* **Source Database** – Raw data storage
* **Destination Database** – Data warehouse
* **Docker Compose** – Container orchestration
* **ELT Script** – Handles extraction, loading, and transformation

---

## ⚙️ Tech Stack

* Docker & Docker Compose
* PostgreSQL
* Python (ELT scripting)
* SQL
* WSL (Windows Subsystem for Linux)
* VS Code

---

## 📂 Project Structure

```
elt/
│
├── docker-compose.yml
├── elt_script.py
├── requirements.txt
├── .env
└── README.md
```

---

## ▶️ Getting Started

### 1️⃣ Clone Repository

```bash
git clone https://github.com/<your-username>/elt-project.git
cd elt-project
```

### 2️⃣ Start Containers

```bash
docker compose up -d
```

### 3️⃣ Check Running Containers

```bash
docker ps
```

### 4️⃣ Access PostgreSQL Container

```bash
docker exec -it elt-destination_postgres-1 psql -U postgres
```

---

## 🔄 ELT Workflow

1. **Extract**
   Data is read from the source PostgreSQL database.

2. **Load**
   Extracted data is loaded into the destination database.

3. **Transform**
   SQL transformations clean and structure the data for analytics.

---

## 🧪 Useful Commands

Start services:

```bash
docker compose up -d
```

Stop services:

```bash
docker compose down
```

View logs:

```bash
docker compose logs
```

---

## 🔐 Environment Variables

Sensitive configuration is stored in `.env` file.

Example:

```
POSTGRES_USER=postgres
POSTGRES_PASSWORD=password
POSTGRES_DB=warehouse
```

⚠️ `.env` file should NO

Example:

```
POSTGRES_USER=postgres
POSTGRES_PASSWORD=password
POSTGRES_DB=warehouse
```

⚠️ `.env` file should NO

# 🖥️ Netdata Monitoring with Docker

## 📊 Project Overview
This project demonstrates how to monitor system and application performance metrics using **Netdata**, an open-source real-time monitoring tool. The setup is done via **Docker**, making it lightweight and easy to run on any machine.

---

## 🎯 Objective
- Install and configure Netdata with Docker  
- Visualize system and container performance metrics  
- Explore alerts, charts, and logs  

---

## 🛠 Tools Used
- **Netdata** (free & open-source monitoring tool)  
- **Docker**  

---

## 🚀 Setup Instructions

### 1️⃣ Run Netdata Container
```bash
docker run -d --name=netdata \
  -p 19999:19999 
````

### 2️⃣ Access the Dashboard

Visit:

```
http://localhost:19999
```

Or if on a remote server:

```
http://<server-ip>:19999
```

---

## 📊 Metrics Monitored

* **CPU usage** (per core, load averages)
* **Memory & Swap** (used, free, cached)
* **Disk I/O** (read/write rates)
* **Network traffic** (bandwidth, errors, packets)
* **Docker containers** (per-container CPU, memory, network)

---

## ⚠️ Alerts & Logs

* Health checks & alerts for CPU, RAM, Disk, and Network
* Logs available via:

```bash
docker logs netdata
```

or inside container:

```bash
cat /var/log/netdata/error.log
```

---

## 📸 Screenshots (to be added)

1. **Docker Container Running**

   <img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/1094c9b0-8586-4a6c-b373-7b429556dde8" />

2. **Netdata Dashboard**

  <img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/764fd600-c058-4127-8f1c-f069069cf809" />


3. **System Metrics Panel**

   <img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/b7ef691c-152b-4e0c-8955-ea3701c396e1" />


---

## ✅ Deliverables

* Live Netdata dashboard running on port **19999**
* Screenshots of container, dashboard, and metrics

---

# 🌐 A Network QoS Monitor System on IP Networks

<p align="center">
  <img src="https://img.shields.io/badge/Program-IISMA_2024-gold?style=for-the-badge" alt="IISMA">
  <img src="https://img.shields.io/badge/Field-Network_Engineering-blue?style=for-the-badge" alt="Field">
  <img src="https://img.shields.io/badge/Location-Taiwan-red?style=for-the-badge" alt="Taiwan, National Formosa University">
</p>

## 🧠 Why I Built This

The increasing reliance on internet services for critical operations highlights the absolute necessity for reliable and high-performing networks. However, network administrators often face structural challenges such as bandwidth limitations, latency, jitter, and packet loss, which significantly impact operational efficiency and user satisfaction.

During my research, I observed that traditional monitoring often lacks the real-time granularity needed to proactively identify issues before they cause service disruptions.
This led to a key objective:

> *How can we implement a robust monitoring system that precisely measures and analyzes key network metrics to ensure optimized reliability in IP networks?* 

---

## 🚀 What I Built

I developed a distributed Quality of Service (QoS) monitoring system that enables institutions to:

* Measure and analyze critical metrics (bandwidth, latency, jitter, and packet loss) in real-time.
* Deploy cost-effective Measurement Agents across various subnets to capture granular data
* Utilize a seamless data pipeline via the MQTT protocol for high-integrity transmission.
* Monitor network health remotely through an interactive, intuitive dashboard
  
This is more than a simple speed test — it is **a real-time network intelligence system for performance optimization.**

---

## 🎯 Project Context

* **Project Type:** GROUP PROJECT (IISMA Research Project)
* **Field:** Network Engineering & IoT.
* **Institution:** National Formosa University (NFU), Taiwan
* **My Role:**  Bandwidth & Latency Lead
* **Validation:** Developed in the IoT and Intelligent Cloud Application Lab under the guidance of Prof. Hui-Kai Su.
---

## 👨‍💻 My Contribution

As part of the group project, I focused on designing and validating the bandwidth and latency measurement workflow, integrating Raspberry Pi-based agents with the monitoring pipeline, and supporting dashboard visualization for real-time and historical QoS analysis.

I also contributed to system testing in the IoT and Intelligent Cloud Application Lab, helping analyze collected data and identify latency bottlenecks despite stable bandwidth performance.

---

## 🌍 System Scale
* Deployed across multiple subnets (A, B, C, D)
* Multiple Raspberry Pi agents collecting data simultaneously
* Real-time data streaming via MQTT protocol
* Continuous monitoring in a real-world lab environment

---

## ⚙️ My Approach (How I Think)

Instead of a centralized, expensive monitoring solution, I focused on three engineering principles:

### 1. Distributed Scalability
Standard monitoring often misses issues occurring in specific network branches.

➡️ I utilized Raspberry Pi 4 devices as agents deployed across Subnets A, B, C, and D to collect precise local data.

### 2. Integration of Hardware & Software
Accurate insights require a seamless bridge between the physical and digital layers.

➡️ I integrated Raspberry Pi 4 hardware with software tools like iPerf3 and MariaDB for structured data management.

### 3. Actionable Visualization
Raw data is complex and often difficult for administrators to interpret quickly.

➡️ I focused on transforming complex metrics into intuitive visual formats, enabling faster decision-making and quicker issue resolution.

---

## 🏗️ System Architecture

<p align="center">
  <img src="Topologi.png" alt="System Architecture" width="500"/>
</p>

<p align="center">
  <em>
The system architecture consists of distributed QoS measurement agents deployed across multiple subnets (A–D) that collect network performance metrics and transmit them via MQTT to a centralized monitoring server integrated with a MariaDB database for storage and analysis. Administrators can remotely access real-time and historical network insights through a web-based dashboard, enabling efficient monitoring and troubleshooting of network performance.
  </em>
</p>

---

## 🚀 Key Features
* **📍 Real-Time QoS Measurement:** Measures bandwidth, latency, jitter, and packet loss using iPerf3.
* **📡 MQTT Communication:** Data transmission via MQTT Broker for real-time distribution and message queuing.
* **📊 Centralized Monitor Server:** A dedicated server that subscribes to topics, validates incoming data, and manages storage.
* **💾 Historical Analysis:** Validated data is stored in MariaDB to facilitate long-term performance auditing.
* **🖥️ Interactive Dashboard:** A real-time web interface providing graphical representations of current and historical network performance.
---

## 🧠 Design Reasoning

### **The Problem: Network Disruptions**
Critical network challenges like bandwidth caps and high latency lead to poor performance and user dissatisfaction.
* **Operational Gap:** Without real-time visibility, administrators cannot proactively resolve issues, leading to reactive maintenance.
  
### **The Solution: Why Agents & MQTT?**
1. **Distributed Measurement:** Raspberry Pi agents allow accurate QoS data collection across different subnet environments.
2. **Data Integrity:** The MQTT protocol maintains consistency and integrity during real-time data reception.
3. **Automated Ecosystem:** Integration of hardware and software replaces manual monitoring workloads with a cohesive, automated system.

---

## Real-World Impact

- **Network Visibility:** The system helped visualize bandwidth, latency, jitter, and packet loss from multiple Raspberry Pi agents in one centralized dashboard.
- **Performance Insight:** Testing revealed that stable bandwidth did not necessarily indicate healthy network performance, as the system uncovered extremely high latency values around 120,000 ms.
- **Operational Efficiency:** The dashboard reduced the need to manually inspect raw network measurements by presenting QoS data in graphs and historical tables.

---

## 📚 Academic Context

This project was developed and documented as part of my IISMA 2024 academic project at National Formosa University.

- **Title:** "A Network QoS Monitor System on IP Networks"
- **Program:** IISMA 2024
- **Institution:** National Formosa University, Taiwan
- **Lab:** IoT and Intelligent Cloud Application Lab
- **Project Certificate:**
<p align="center">
  <img src="Achmad Doli Harahap_Sertifikat Project IISMA_page-0001.jpg" alt="IISMA 2024 Certificate" width="350px"/>
</p>

---

## 🛠️ Tech Stack
| Category | Tools & Technologies |
| :--- | :--- |
| **Hardware** | Raspberry Pi 4 Model B, TP-Link AC1750 |
| **Backend** | Python, MariaDB (MySQL), MQTT (Mosquitto) |
| **Network Tools**| iPerf3 (Traffic Analysis), MQTT Protocol |
| **Visualization**|  Real-Time Dashboard with Graphical Representation |

---

## 🔄 Full System Workflow

### 1. System Architecture
1. **Agent Initialization:** Raspberry Pi configures hardware and software.
2. **Measurement:** Agents measure QoS parameters using iPerf3.
3. **Transmission:** Validated and formatted data is published to the **MQTT Broker**.
4. **Processing:** The **QoS Monitor Server** subscribes to relevant topics, validates the data, and stores it in **MariaDB**.
5. **Visualization:** The **Real-Time Dashboard** processes the database records to update intuitive graphs and tables.
   
---

## 🌐 Live System Access
You can explore the live monitoring dashboard directly through the link below:
- **Dashboard Link:** [QoS Monitoring Dashboard](https://hksu.ee.nfu.edu.tw/netqos/webqos/dashboard/index.php)

**Username**: 
doli

**Password**: 
doli

---

## 📺 Visuals & Simulation

### 💻 Dashboard Interface
*The dashboard provides clear insights into network performance across multiple Raspberry Pi agents.*

<p align="center">
  <img src="Dashboard.png" alt="QoS Trend Graphs Raspberry Pi 1" width="48%"/>
  <img src="Dashboard kedua.png" alt="QoS Trend Graphs Raspberry Pi 2" width="48%"/>
</p>

<p align="center">
  <img src="Data Raspberry 1.png" alt="QoS Data Raspberry Pi 1" width="48%"/>
  <img src="Data Raspberry 2.png" alt="QoS Data Raspberry Pi 2" width="48%"/>
</p>

<p align="center">
  <em>
  The dashboard visualizes real-time QoS trends from Raspberry Pi 1 and Raspberry Pi 2, while the data tables show raw QoS records collected from each agent for comparative analysis across distributed network nodes.
  </em>
</p>

### 🎥 Video Demonstration
*Click the thumbnail below to watch the system in action.*

#### **Real-Time QoS Monitoring Simulation**
[![QoS Monitoring Demo](https://img.youtube.com/vi/yh7UTDM0ioo/0.jpg)](https://youtu.be/yh7UTDM0ioo?si=g5CrX00akOpRSh4s)

> **Simulation Focus:**  
> Demonstrates real-time QoS data collection from distributed Raspberry Pi agents, including bandwidth, latency, jitter, and packet loss, along with data transmission via MQTT and visualization on the monitoring dashboard.

---

## 📊 Key Findings

- Stable bandwidth performance (~1 Mbps)
- Extremely high latency (~120,000 ms)

🚨 Insight:
The system revealed a critical network bottleneck, showing that stable bandwidth does not guarantee low latency, highlighting the need for deeper QoS monitoring in real-world environments.

---

## 📈 Learning Journey

### **⚠️ Challenges & How I Overcame Them**
1. **Data Inconsistencies**
   * **Challenge:** During reception, some data packets might be inconsistent or contain errors.
   * **Solution:** I implemented a Data Validation phase at the server level, logging invalid data for debugging to ensure only accurate metrics are stored and visualized.
     
### **What I Learned**

Working at the IoT and Intelligent Cloud Application Lab in Taiwan strengthened my understanding of distributed monitoring systems, QoS metrics, and real-time data pipelines. I learned how to validate bandwidth and latency measurements, interpret network performance anomalies, and transform raw network data into actionable insights through dashboard visualization.

---


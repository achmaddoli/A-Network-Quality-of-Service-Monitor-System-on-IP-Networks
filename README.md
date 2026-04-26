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
  
This is more than a simple speed test — it is a foundation for network performance optimization.

---

## 🎯 Project Context

* **Type:** International Student Project (IISMA 2024)
* **Field:** Network Engineering & IoT.
* **Institution:** National Formosa University (NFU), Taiwan
* **Validation:** Developed in the IoT and Intelligent Cloud Application Lab under the guidance of Prof. Hui-Kai Su.
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

## 🚀 Key Features
* **📍Real-Time Tracking:** Precise measurement of bandwidth, latency, jitter, and packet loss using iPerf3.
* **📡 MQTT Communication:** Data transmission via MQTT Broker for real-time distribution and message queuing.
* **📊 Centralized Monitor Server:** A dedicated server that subscribes to topics, validates incoming data, and manages storage.
* **💾 Historical Analysis:** Validated data is stored in MariaDB to facilitate long-term performance auditing.
* **🖥️ Interactive Dashboard:** A real-time web interface providing graphical representations of current and historical network performance.
---

## 🧠 Comprehensive Reasoning (The "Why")

### **The Problem: Network Disruptions**
Critical network challenges like bandwidth caps and high latency lead to poor performance and user dissatisfaction.
* **Operational Gap:** Without real-time visibility, administrators cannot proactively resolve issues, leading to reactive maintenance.
  
### **The Solution: Why Agents & MQTT?**
1. **Precision Logic:** Precision Logic: Distributed agents allow for accurate data collection across a diverse network configuration.
2. **Data Integrity:** The MQTT protocol maintains consistency and integrity during real-time dataReception.
3. **Automated Ecosystem:** Integration of hardware and software replaces manual monitoring workloads with a cohesive, automated system.

---

## Real-World Impact
- **Network Reliability**: Administrators can proactively identify and resolve network issues, significantly enhancing user satisfaction.
- **Efficiency**: Transforming complex network data into actionable insights through clear visualization.

---

## 📚 Academic Achievement
The methodology and results of this project were peer-reviewed and documented:
- Title: "A Network QoS Monitor System on IP Networks".
- Award: IISMA 2024 Project Completion at National Formosa University.

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
1. **Agent Initialization:** Agen Raspberry Pi menyiapkan konfigurasi *hardware* dan *software*[cite: 30].
2. **Measurement:** Agen mengukur parameter QoS menggunakan iPerf3[cite: 31].
3. **Transmission:** Data yang divalidasi dan diformat dipublikasikan ke **MQTT Broker**[cite: 37].
4. **Processing:** **QoS Monitor Server** berlangganan topik terkait, memvalidasi data, dan menyimpannya di **MariaDB**[cite: 48, 54].
5. **Visualization:** **Real-Time Dashboard** memproses catatan database untuk memperbarui grafik dan tabel yang intuitif[cite: 55].

---

## 📺 Visuals & Simulation

### 💻 Dashboard Interface
*Dashboard memberikan wawasan yang jelas tentang kinerja jaringan di seluruh subnet.*

| 📊 QoS Data Records | 📡 Real-Time Trend Graphs |
| :---: | :---: |
|  |  |
| [cite_start]*Tampilan tabel metrik mentah dari Agen Pi* [cite: 137] | [cite_start]*Tren visual untuk Bandwidth, Latency, dan Jitter* [cite: 178] |

---

## 📈 Learning Journey

### **⚠️ Challenges & Overcoming Them**
1. **Data Inconsistencies**
   * **Challenge:** Selama penerimaan, beberapa paket data mungkin tidak konsisten atau mengandung kesalahan.
   * [cite_start]**Overcoming:** Saya mengimplementasikan fase **Validasi Data** di tingkat server, mencatat data yang tidak valid untuk *debugging* guna memastikan hanya metrik akurat yang disimpan dan divisualisasikan[cite: 50, 51].

### **What I Learned**
[cite_start]Bekerja di **IoT and Intelligent Cloud Application Lab** di Taiwan mengasah keterampilan saya dalam **Integrasi Data dan Pemecahan Masalah Tingkat Lanjut**[cite: 79, 81]. [cite_start]Saya belajar menguasai integrasi *hardware* Raspberry Pi 4 dengan alat *software* yang kokoh, mengembangkan pemahaman komprehensif tentang sinkronisasi sistem *real-time*[cite: 63, 69]. [cite_start]Di luar keterampilan teknis, bekerja di lingkungan multidisiplin mengembangkan kemampuan **Collaborative Development** saya[cite: 82].

---
*Developed with ❤️ during IISMA at National Formosa University*

# 🌐 A Network QoS Monitor System on IP Networks

<p align="center">
  <img src="https://img.shields.io/badge/Program-IISMA_2024-gold?style=for-the-badge" alt="IISMA">
  <img src="https://img.shields.io/badge/Field-Network_Engineering-blue?style=for-the-badge" alt="Field">
  <img src="https://img.shields.io/badge/Location-Taiwan-red?style=for-the-badge" alt="Taiwan, National Formosa University">
</p>

## 🧠 Why I Built This

[cite_start]Ketergantungan yang semakin tinggi pada layanan internet untuk operasi kritis menuntut jaringan yang andal dan berkinerja tinggi[cite: 8]. [cite_start]Namun, tantangan utama seperti **keterbatasan bandwidth, latency, jitter, dan packet loss** sering kali menjadi hambatan besar yang menurunkan kepuasan pengguna dan efisiensi operasional[cite: 9].

Selama masa studi saya di Taiwan, saya mengamati bahwa pemantauan jaringan tradisional sering kali kurang memiliki detail *real-time* yang dibutuhkan untuk mengidentifikasi masalah secara proaktif.

Hal ini memicu pertanyaan kunci:

> [cite_start]*Bagaimana kita bisa membangun sistem pemantauan yang kokoh untuk mengukur metrik jaringan secara presisi demi menjamin reliabilitas pada jaringan IP?* [cite: 10]

---

## 🚀 What I Built

Saya mengembangkan **ekosistem pemantauan QoS (Quality of Service) terdistribusi** yang memungkinkan administrator jaringan untuk:

* [cite_start]Mengukur dan menganalisis metrik kritis (**Bandwidth, Latency, Jitter, dan Packet Loss**) secara *real-time*[cite: 72].
* [cite_start]Menyebarkan **Measurement Agents** yang hemat biaya di berbagai subnet untuk menangkap data yang granular[cite: 65, 73].
* [cite_start]Memanfaatkan pipa data yang mulus melalui protokol **MQTT** untuk transmisi data berintegritas tinggi[cite: 25, 45].
* [cite_start]Memantau kesehatan jaringan dari jarak jauh melalui **dashboard interaktif dan intuitif**[cite: 76].

[cite_start]Ini lebih dari sekadar tes kecepatan biasa — ini adalah **fondasi untuk optimasi kinerja jaringan**[cite: 68, 70].

---

## 🎯 Project Context

* [cite_start]**Type:** International Student Project (IISMA 2024)[cite: 6].
* [cite_start]**Field:** Network Engineering & IoT[cite: 2, 242].
* [cite_start]**Institution:** National Formosa University (NFU), Taiwan[cite: 222, 242].
* **Validation:** Dikembangkan di **IoT and Intelligent Cloud Application Lab** di bawah bimbingan **Prof. [cite_start]Hui-Kai Su**[cite: 242, 189].

---

## ⚙️ My Approach (How I Think)

Alih-alih menggunakan solusi pemantauan terpusat yang mahal, saya berfokus pada tiga prinsip rekayasa:

### 1. Distributed Scalability
Pemantauan standar sering melewatkan masalah yang terjadi di cabang jaringan tertentu.
[cite_start]➡️ Saya menggunakan perangkat **Raspberry Pi 4 sebagai agen** yang ditempatkan di berbagai subnet (A, B, C, D) untuk mengumpulkan data lokal yang presisi[cite: 24, 65].

### 2. Integration of Hardware & Software
Wawasan yang akurat membutuhkan jembatan yang mulus antara lapisan fisik dan digital.
[cite_start]➡️ Saya mengintegrasikan *hardware* **Raspberry Pi 4** dengan alat *software* seperti **iPerf3** dan **MariaDB** untuk manajemen data yang terstruktur[cite: 79].

### 3. Actionable Visualization
Data mentah sering kali sulit diinterpretasikan dengan cepat oleh administrator.
[cite_start]➡️ Saya berfokus pada transformasi metrik kompleks menjadi **format visual yang intuitif**, memungkinkan pengambilan keputusan dan penyelesaian masalah yang lebih cepat[cite: 80].

---

## 🚀 Key Features
* [cite_start]**📊 Real-Time Tracking:** Pengukuran presisi bandwidth, latency, jitter, dan packet loss menggunakan iPerf3[cite: 31, 69].
* **📡 MQTT Communication:** Transmisi data via MQTT Broker untuk distribusi *real-time* dan pengantrean pesan[cite: 37, 43, 45].
* [cite_start]**📊 Centralized Monitor Server:** Server khusus yang berlangganan topik, memvalidasi data masuk, dan mengelola penyimpanan[cite: 46, 50].
* [cite_start]**💾 Historical Analysis:** Data yang divalidasi disimpan di **MariaDB** untuk memfasilitasi audit kinerja jangka panjang[cite: 54].
* **🖥️ Interactive Dashboard:** Antarmuka web *real-time* yang menyediakan representasi grafis dari kinerja jaringan saat ini dan historis[cite: 55, 60].

---

## 🧠 Comprehensive Reasoning (The "Why")

### **The Problem: Network Blind Spots**
Tantangan jaringan seperti batasan bandwidth dan latency tinggi menyebabkan kinerja buruk dan ketidakpuasan pengguna[cite: 9].
* [cite_start]**Operational Gap:** Tanpa visibilitas *real-time*, administrator tidak dapat menyelesaikan masalah secara proaktif, yang berujung pada pemeliharaan yang bersifat reaktif[cite: 64].

### **The Solution: Why Agents & MQTT?**
1. [cite_start]**Precision Logic:** Agen terdistribusi memungkinkan pengumpulan data yang akurat di seluruh konfigurasi jaringan yang beragam[cite: 63].
2. [cite_start]**Data Integrity:** Protokol **MQTT** menjaga konsistensi dan integritas selama penerimaan data secara *real-time*[cite: 45].
3. [cite_start]**Automated Ecosystem:** Integrasi *hardware* dan *software* menggantikan beban kerja pemantauan manual dengan sistem yang kohesif dan otomatis[cite: 69].

---

## 🛠️ Tech Stack
| Category | Tools & Technologies |
| :--- | :--- |
| **Hardware** | [cite_start]Raspberry Pi 4 Model B, TP-Link AC1750[cite: 273, 276]. |
| **Backend** | [cite_start]Python, MariaDB (MySQL), MQTT (Mosquitto)[cite: 280, 289, 292]. |
| [cite_start]**Network Tools**| iPerf3 (Traffic Analysis), MQTT Protocol[cite: 277, 286]. |
| **Visualization**| [cite_start]Real-Time Dashboard with Graphical Representation[cite: 271]. |

---

## 🔄 Full System Workflow

### 1. System Architecture
1. [cite_start]**Agent Initialization:** Agen Raspberry Pi menyiapkan konfigurasi *hardware* dan *software*[cite: 30].
2. [cite_start]**Measurement:** Agen mengukur parameter QoS menggunakan iPerf3[cite: 31].
3. [cite_start]**Transmission:** Data yang divalidasi dan diformat dipublikasikan ke **MQTT Broker**[cite: 37].
4. [cite_start]**Processing:** **QoS Monitor Server** berlangganan topik terkait, memvalidasi data, dan menyimpannya di **MariaDB**[cite: 48, 54].
5. [cite_start]**Visualization:** **Real-Time Dashboard** memproses catatan database untuk memperbarui grafik dan tabel yang intuitif[cite: 55].

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

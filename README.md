# 🛡️ ARP Sentinel – Real-time MITM & Gateway Protection

**ARP Sentinel** adalah aplikasi keamanan jaringan berbasis **real-time monitoring** yang dirancang untuk **mendeteksi, mencegah, dan memitigasi serangan ARP Poisoning, Man-In-The-Middle (MITM), dan Gateway Denial of Service** pada jaringan LAN dan WiFi.

Aplikasi ini berfokus pada **defensive security**, bukan serangan balik, dengan pendekatan **lock, verify, and monitor** terhadap protokol ARP yang secara default bersifat trusting.

---

## 🖥️ Tampilan Aplikasi

![ARP Sentinel Interface](assets/ARP%20Sentinel.png)

Antarmuka ARP Sentinel menampilkan informasi penting secara real-time, seperti:

* IP Address & MAC Address aktif
* Vendor perangkat
* Status client & gateway
* MITM confidence score
* Monitoring gateway (online/offline)

Tampilan ini membantu pengguna **mengidentifikasi anomali jaringan dengan cepat dan akurat**.

---

## 🚨 Masalah yang Diselesaikan

Protokol ARP tidak memiliki mekanisme autentikasi. Akibatnya, jaringan rentan terhadap:

* ARP Poisoning / ARP Spoofing
* Man-In-The-Middle (MITM)
* Session Hijacking
* Credential Sniffing
* Kill Connection / Gateway DoS

Serangan-serangan ini sering dilakukan menggunakan tools seperti:

* Cain & Abel
* Ettercap / Bettercap
* Netcut / Arcai Netcut
* WiFiKill
* Custom Python scripts (scapy, arpspoof)

---

## ✅ Solusi: ARP Sentinel

ARP Sentinel menutup celah tersebut dengan **proteksi aktif** terhadap ARP Table dan Gateway, sehingga serangan di atas menjadi **tidak efektif**.

---

## 🔑 Fitur Utama

### 🔒 Static ARP Lock

Mengunci relasi **IP ↔ MAC Address** gateway dan host, mencegah ARP palsu masuk ke sistem.

### 📡 Gratuitous ARP Pulse

Mengirim ARP legitimate secara berkala untuk:

* Menegaskan identitas asli ke router
* Menjaga konsistensi ARP cache
* Mengacaukan ARP spoofing penyerang

### 🧠 Gateway Watchdog

Memantau respon gateway secara real-time dan mendeteksi:

* Gateway hijacking
* Kill connection attack
* Partial DoS

### ⚠️ MITM Confidence Scoring

Menilai tingkat ancaman MITM dalam persentase (0–100%) berdasarkan anomali ARP & gateway behavior.

---

## 🧩 Fitur Tambahan

* **Auto-Kill Switch**
  Memutus koneksi internet secara otomatis jika MITM terdeteksi pada level kritis untuk mencegah kebocoran data.

* **Restore Connection**
  Mengaktifkan ulang adapter jaringan (Wi-Fi/Ethernet) dan mengembalikan koneksi ke kondisi normal.

* **Ultra Stealth Mode**

  * Membersihkan ARP cache
  * Menyembunyikan host dari ARP scanner
  * Mengurangi fingerprint jaringan

---

## 🧪 Ancaman yang Terbukti Terblokir

| Serangan              | Status      |
| --------------------- | ----------- |
| ARP Poisoning         | ✅ Blocked   |
| MITM LAN              | ✅ Blocked   |
| Netcut / WiFiKill     | ✅ Mitigated |
| Sniffing via Spoofing | ✅ Prevented |
| Gateway DoS           | ✅ Detected  |

---

## 🛠️ Platform & Lingkungan

* **OS**: Windows
* **Network**: LAN / WiFi
* **Mode**: Passive Defense
* **Target User**:

  * Network Administrator
  * IT Support
  * Cyber Security Enthusiast
  * Home / Office Users

---

## ⚠️ Disclaimer

ARP Sentinel adalah **alat defensive security**.
Aplikasi ini **tidak digunakan untuk menyerang, menyadap, atau mengganggu jaringan lain**.

Gunakan hanya pada:

* Jaringan milik sendiri
* Jaringan dengan izin resmi

---

## 🤝 Kontribusi

Kontribusi sangat terbuka:

* Bug report
* Feature request
* Code improvement
* Dokumentasi

Silakan buat **Issue** atau **Pull Request**.

---

## 📄 Lisensi

Proyek ini menggunakan lisensi **MIT License**.
Bebas digunakan, dimodifikasi, dan didistribusikan dengan tetap menyertakan atribusi.

---

## ⭐ Dukungan

Jika project ini membantu:

* ⭐ Star repository ini
* 🍴 Fork untuk pengembangan
* 📢 Bagikan ke komunitas keamanan jaringan

---

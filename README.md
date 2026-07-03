# tugas-jaringan-komputer

Repositori ini berisi kumpulan proyek simulasi arsitektur jaringan yang saya kembangkan untuk mendemonstrasikan implementasi infrastruktur IT pada skala *enterprise* dan *smart retail*. 

Semua proyek di bawah ini dibangun sebagai **Proof of Concept (PoC)** dengan fokus pada desain topologi logis, segmentasi jaringan, dan integrasi keamanan.

---

## 📌 Daftar Proyek
1. [Enterprise Game Server Architecture (GNS3)](#1-enterprise-game-server-architecture)
2. [Smart Retail Network & IoT Integration (Packet Tracer)](#2-smart-retail-network--iot-integration)

---

## 1. Enterprise Game Server Architecture
**Tools:** GNS3, Fortigate (Firewall), HAProxy (Load Balancer), VLAN, CDN Server  
**Folder:** `/enterprise-game-server-gns3`

### Deskripsi Proyek
Proyek ini adalah *Proof of Concept* (PoC) untuk merancang infrastruktur jaringan server *game online* internasional. Fokus utama dari arsitektur ini adalah penerapan keamanan *multi-tier* dengan memisahkan secara logis antara server publik (Game & CDN) dan server internal (Data User).

### Sorotan Arsitektur & Konfigurasi
*   **Security Perimeter:** Implementasi Fortigate Firewall untuk memfilter trafik masuk dan melindungi infrastruktur internal.
*   **Multi-Tier Architecture:** Pemisahan server data pengguna dari server game publik untuk meminimalisir risiko kebocoran data.
*   **Content Delivery:** Integrasi *single-node* CDN untuk menyimulasikan distribusi konten (aset game) ke pengguna.
*   **Load Balancing (PoC):** Penyiapan *node* HAProxy untuk distribusi beban trafik. *(Catatan: Karena keterbatasan sumber daya komputasi/hardware constraints pada lingkungan simulasi lokal, pengujian load balancing HAProxy tidak dilakukan secara ekstensif).*

### Topologi Jaringan
![Topologi GNS3](perusahaan-game-gns3/Topologi-Jaringan.png)
*(Tambahkan penjelasan singkat 1-2 kalimat di bawah gambar jika perlu)*

---

## 2. Smart Retail Network & IoT Integration
**Tools:** Cisco Packet Tracer, Cisco IOS, IoT Devices  
**Folder:** `/smart-retail-packet-tracer`

### Deskripsi Proyek
Merancang dan mensimulasikan infrastruktur jaringan modern untuk lingkungan ritel cerdas (*smart retail*). Proyek ini mendemonstrasikan bagaimana perangkat IoT dapat diintegrasikan secara aman ke dalam jaringan korporat menggunakan segmentasi jaringan.

### Sorotan Arsitektur & Konfigurasi
*   **Network Segmentation (VLAN):** Mengisolasi trafik antara operasional toko, perangkat IoT, dan manajemen jaringan untuk meningkatkan keamanan.
*   **Inter-VLAN Routing:** Mengimplementasikan metode *Router-on-a-Stick* untuk memungkinkan komunikasi antar segmen jaringan secara terkendali.
*   **IoT Automation:** Mengonfigurasi dan menghubungkan berbagai perangkat sensor ritel (IoT) ke dalam satu ekosistem jaringan terpusat.

### Topologi Jaringan
![Topologi Packet Tracer](ritel-pintar-packet-tracer/Topologi-Jaringan.png)
*(Tambahkan penjelasan singkat 1-2 kalimat di bawah gambar jika perlu)*

---

## 🚀 Cara Menggunakan Repositori Ini
Setiap proyek memiliki foldernya masing-masing. Di dalam folder tersebut, Anda dapat menemukan:
*   File simulasi (`.gns3` atau `.pkt`)
*   Dokumentasi pendukung dan laporan analisis
*   Folder `configs/` yang berisi teks konfigurasi mentah (*raw config*) dari perangkat jaringan yang digunakan.

## 📬 Kontak
Mari terhubung di [LinkedIn](masukkan-link-linkedin-kamu-di-sini) untuk berdiskusi lebih lanjut mengenai jaringan dan keamanan siber!
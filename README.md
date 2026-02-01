# 🏛️ EKOSISTEM DIGITAL MASJID KAMPUNG SUNGAI LANG BARU (MKSLB)
> **Sesi Pentadbiran 2026 / 2030**

Selamat datang ke pusat dokumentasi dan pengurusan digital rasmi **MKSLB**. Repository ini berfungsi sebagai pusat rujukan (Ensiklopedia) dan integrasi bagi semua sistem aplikasi yang menyokong pengurusan masjid secara sistematik.

---

## 🎯 Visi & Misi Digital
* **Visi:** Menjadikan MKSLB sebagai model Masjid Pintar (Smart Masjid) yang telus dan efisien di daerah Kuala Langat.
* **Misi:** Mengintegrasikan teknologi awan (Cloud) dan API untuk memudahkan urusan kehadiran, pengurusan takwim, dan laporan aktiviti biro.

---

## 🏗️ Arsitektur Ekosistem (Visi Perlaksaan)

Berikut adalah gambaran bagaimana setiap komponen digital yang kita bina saling berhubung kait:

```mermaid
graph TD
    A[🏛️ Portal Pusat MKSLB] --> B[📅 API Takwim Solat]
    A --> C[📝 Sistem Kehadiran]
    
    subgraph "Data & API"
    B --> B1[GitHub Pages JSON]
    B1 --> B2[Kiosk TV / Dashboard]
    end

    subgraph "Sistem Kehadiran"
    C --> C1[Petugas Solat 5 Waktu]
    C --> C2[Mesyuarat AJK & Biro]
    end

    subgraph "Penyimpanan Rekod"
    C1 & C2 --> D[Google Apps Script]
    D --> E[📊 Google Sheets Master]
    end

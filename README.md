# uas-commproto-kelompok-6

Repositori ini dibuat untuk memenuhi tugas Ujian Akhir Semester (UAS) Genap T.A. 2025/2026 pada program studi Sains Data, Universitas Cakrawala. Project ini mengimplementasikan protokol komunikasi REST API untuk melakukan ingestion data (dataset skala kecil) yang dilengkapi dengan pengujian automated, analisis trafik, serta pemantauan log (observability).

## 👥 Anggota Kelompok & Peran
* **25110500015 - Azka Artie Rabbani** — **Role 1: API & Postman Tester** (Mendesain endpoint, request success/error, automated testing)
* **25110500018 - Kanaya Anantani Syafikri** — **Role 2: Protocol & Traffic Analyst** (Analisis protokol Wireshark, header/payload, network flow)
* **25110500024 - Wandasari Tunggul Hadi Kusumo Astuti** — **Role 3: Integration/Workflow Engineer** (Menghubungkan komponen, mock service/n8n integration, logging)
* **251105000 - Olga Rizky Ramadhani** — **Role 4: Documentation & Presenter Lead** (Penyusunan laporan, PPT, README, tata kelola repositori)

---

## 🛠️ Ringkasan Use Case & Cakupan
* **Use Case:** API Ingestion Dataset (REST + Postman)
* **Deskripsi:** Sistem menerima dataset kecil berupa data JSON/CSV, memvalidasi struktur data, dan menghasilkan respons yang sesuai (Success/Error).
* **Komponen Arsitektur:**
    * **Client:** Postman / cURL
    * **Entry Point / Processing:** API Server Lokal (Python Flask / FastAPI / Mock Server)
    * **Output/Observability:** Application Log & Wireshark Traffic Capture

---

## 📐 Arsitektur & Alur Data (Data Flow)

### 1. Architecture Canvas

[Client: Postman] ---> [Entry Point: REST API Server] ---> [Processing & Validation] ---> [Logging / Output]


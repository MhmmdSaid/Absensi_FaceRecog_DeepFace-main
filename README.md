# 🧠 DeepFace Attendance System (Telkomsat Internship)

Sistem Absensi Wajah berbasis **FastAPI + DeepFace + PostgreSQL (pgvector)**  
dengan dukungan **Liveness Detection (Blink Detection)** menggunakan **MediaPipe FaceMesh**.

---

## 🚀 Fitur Utama

✅ Deteksi wajah otomatis dengan DeepFace  
✅ Verifikasi liveness (kedipan 2x) sebelum absensi  
✅ Upload dataset wajah baru (manual collector)  
✅ Indexing otomatis dan manajemen database wajah  
✅ Integrasi PostgreSQL + pgvector untuk similarity search  
✅ Dashboard frontend modern berbasis TailwindCSS  

---

## 🏗️ Struktur Folder

deepface_attendance/
│
├── backend/
│ ├── main.py # FastAPI backend utama
│ ├── setup_tables.py # Pembuatan tabel database
│ ├── index_data.py # Indexing dataset wajah → pgvector
│ ├── utils.py # Ekstraksi fitur wajah (DeepFace)
│ ├── interns.csv # Metadata peserta internship
│ └── requirements.txt # Dependensi Python
│
├── frontend/
│ ├── main.html # Halaman absensi (dengan kedipan)
│ ├── data.html # Data absensi hari ini
│ ├── data_collector.html # Upload dataset wajah
│ ├── settings.html # Sinkronisasi & indexing manual
│ ├── main.js # Liveness + absensi
│ ├── data.js # Tabel data absensi
│ ├── data_collector.js # Upload dataset
│ ├── settings.js # Sinkronisasi dan manajemen wajah
│ ├── style.css # Styling utama (Tailwind + custom)
│ └── png/ # Ikon & logo
│
├── docker-compose.yml # Konfigurasi Docker multi-service
├── Dockerfile # Build image FastAPI
└── README.md # Dokumentasi proyek ini

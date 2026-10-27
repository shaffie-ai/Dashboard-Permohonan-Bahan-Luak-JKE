# ⚡ Dashboard Permohonan Bahan Luak JKE

Sistem pengurusan permohonan bahan luak untuk Jabatan Kejuruteraan Elektrik (JKE) — dibina dengan React, Vite, dan Supabase.

---

## 📁 Struktur Fail

​```
jke-web/
├── src/
│   ├── pages/
│   │   ├── LoginPage.jsx         ← Halaman log masuk
│   │   ├── DaftarPage.jsx        ← Halaman daftar akaun
│   │   ├── HomePensyarah.jsx     ← Dashboard utama pensyarah
│   │   ├── BorangPermohonan.jsx  ← Borang permohonan bahan luak
│   │   ├── SenaraiPermohonan.jsx ← Senarai & status permohonan
│   │   └── DashboardKoordinator.jsx ← Dashboard penyelaras perolehan
│   ├── components/
│   │   ├── Navbar.jsx            ← Bar navigasi
│   │   ├── StatusBadge.jsx       ← Badge warna status
│   │   └── ProgressTracker.jsx   ← Tracker status permohonan
│   ├── lib/
│   │   ├── supabase.js           ← Konfigurasi Supabase
│   │   └── supabase-setup.sql    ← SQL setup database
│   └── App.jsx                   ← Root app & routing
├── .env.example                  ← Contoh konfigurasi environment
├── .gitignore
├── package.json
└── vite.config.js
​```

---

## 🚀 Cara Guna

### 1. Clone repositori ini
​```bash
git clone https://github.com/shaffie-ai/Dashboard-Permohonan-Bahan-Luak.git
cd jke-web
​```

### 2. Install dependencies
​```bash
npm install
​```

### 3. Setup environment variable
​```env
VITE_SUPABASE_URL=https://XXXXXXXXXXXX.supabase.co
VITE_SUPABASE_ANON_KEY=your-anon-key-here
​```

### 4. Setup database Supabase
- Log masuk ke [supabase.com](https://supabase.com)
- Buka **SQL Editor** → jalankan fail `src/lib/supabase-setup.sql`

### 5. Jalankan aplikasi
​```bash
npm run dev
​```

---

## ✨ Ciri-ciri

### 👨‍🏫 Pensyarah
- ✅ Log masuk menggunakan Gmail
- ✅ Isi borang permohonan bahan luak
- ✅ Semak status permohonan dengan progress tracker
- ✅ Notifikasi status: Menunggu → Dikompil → Dalam Perolehan → Diterima

### 📊 Koordinator Perolehan
- ✅ Dashboard semua permohonan dari 40 pensyarah
- ✅ Kemaskini status permohonan
- ✅ Kompilasi automatik bahan yang sama dari pelbagai pensyarah
- ✅ Export senarai perolehan ke CSV

---

## 🛠️ Teknologi

| Teknologi | Kegunaan |
|-----------|----------|
| [React](https://react.dev) | Frontend framework |
| [Vite](https://vitejs.dev) | Build tool |
| [Supabase](https://supabase.com) | Database & Authentication |
| [React Router](https://reactrouter.com) | Routing |

---

## 👥 Pengguna

- **Pensyarah** — 40 orang, boleh buat dan semak permohonan sendiri
- **Koordinator** — 1 orang, boleh lihat semua permohonan dan kemaskini status

---

*Jabatan Kejuruteraan Elektrik (JKE)*

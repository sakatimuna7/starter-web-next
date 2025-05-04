# 🚀 Next.js Custom Template – Newus PR Boilerplate

Selamat datang di proyek berbasis **Next.js** dengan kustomisasi internal dari tim Newus Technology. Template ini menggunakan boilerplate `pr-template-nextjs` sebagai fondasi utama, dikembangkan untuk mempercepat pengembangan aplikasi web yang modern, cepat, dan scalable.

---

## 📁 Struktur Folder

```bash
.
├── public/                 # Static assets
├── src/
│   ├── components/         # Reusable components (UI, layouts, modals, etc.)
│   ├── constants/          # Global constants (e.g., routes, configs)
│   ├── context/            # React context providers
│   ├── hooks/              # Custom React hooks
│   ├── lib/                # Utility functions or API wrappers
│   ├── pages/              # Next.js page routing
│   ├── services/           # API service layers (axios/fetch)
│   ├── styles/             # Global styles, Tailwind config
│   ├── types/              # TypeScript interfaces and types
│   └── utils/              # Helper utilities
├── .env.example            # Contoh environment config
├── next.config.js          # Next.js config
├── tailwind.config.js      # Tailwind CSS config
└── README.md               # Dokumentasi proyek
```

---

## ⚙️ Teknologi dan Library

- **Framework**: Next.js (App Router / Pages Router)
- **Styling**: Tailwind CSS + Custom Theme
- **State Management**: React Context / Zustand
- **Form Handling**: React Hook Form + Yup
- **HTTP Client**: fetch bawaan dengan custom fetching
- **UI Component**: shadcn/ui (Headless UI + Radix UI)
- **Icon Library**: lucide-react
- **Linting**: ESLint, Prettier, Husky
- **CI/CD Ready**: GitHub Actions
- **Deployment**:  VPS

---

## 🧑‍💻 Cara Menjalankan Project

### 1. Clone Repositori

```bash
git clone https://github.com/nama-user/nama-repo.git
cd nama-repo
```

### 2. Install Dependency

```bash
pnpm install
```

### 3. Buat file `.env.local`

```bash
cp .env.example .env.local
```

Isi konfigurasi sesuai environment Anda (lihat bagian `.env` di bawah).

### 4. Jalankan di Lokal

```bash
pnpm dev
```

Akses aplikasi di: [http://localhost:3000](http://localhost:3000)

---

## 🔐 Environment Variable (.env)

| Key                  | Keterangan                              |
| -------------------- | --------------------------------------- |
| NEXT_PUBLIC_API_URL  | Base URL untuk API backend              |



---

## ✅ Standar Kode

- Gunakan `pnpm lint` sebelum push
- Format otomatis dengan Prettier: `pnpm format`
- Konvensi commit menggunakan [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
- Gunakan `GitHub Pull Request` untuk semua perubahan (auto lint & test via CI)

---

## 📦 Fitur Khusus Template

- ✅ Autentikasi JWT (client-side & server-side protection)
- ✅ Layout dinamis (dengan metadata Head otomatis)
- ✅ Konfigurasi akses role-based (Admin/User)
- ✅ Dark mode siap pakai (opsional)
- ✅ Komponen modal, toast, alert dialog custom
- ✅ Global loading & error boundary
- ✅ Integrasi socket.io siap (jika diperlukan)

---

## 🧪 Testing (Opsional)

```bash
# Unit test dengan Vitest atau Jest
pnpm test
```

---

## 🚀 Deployment

- Pastikan variabel `.env` sudah disesuaikan untuk production.
- Untuk deploy ke **Vercel**:
  - Connect GitHub repository.
  - Pastikan env key di-setting via dashboard.
- Untuk VPS, gunakan build + serve:

```bash
pnpm build
pnpm start
```

---

## 📋 Lisensi

Open Source

---

## ✨ Credits

Template ini di setup oleh @sakatimuna7 dan kolaborasi oleh @aldngrha

---

## 🙋 FAQ

**Q: Bisa digunakan untuk proyek publik?**  
A: Ya, namun direkomendasikan untuk proyek private atau internal dengan flow tim terstruktur.


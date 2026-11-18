# 💪 Panduan UL-UL untuk Pemula

Panduan latihan Upper-Lower (UL-UL) untuk pemula. Versi ringan: 4 hari gym/kardio rendah dampak tanpa lari, selama lutut kanan dipulihkan.

## 🌐 Akses Online

Setelah deploy ke GitHub Pages, akses di:
```
https://<username>.github.io/workout-plan/
```

## ✨ Fitur

- 📱 **PWA (Progressive Web App)** - Bisa di-install di HP seperti app native
- 🌙 **Dark/Light Mode** - Otomatis mengikuti sistem atau toggle manual
- 🎬 **Animasi SVG** - Animasi gerakan gym dengan muscle highlight
- 📊 **Scroll Progress** - Indikator progress scroll
- 🔄 **Offline Support** - Bisa diakses tanpa internet setelah pertama kali dibuka
- 📱 **Responsive** - Optimal di semua ukuran layar
- ♿ **Accessible** - Mendukung reduced motion dan screen readers

## 🚀 Deploy ke GitHub Pages

### Cara 1: GitHub Actions (Otomatis)

1. Push ke GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/<username>/workout-plan.git
   git push -u origin main
   ```

2. Di GitHub → Settings → Pages → Source: pilih **GitHub Actions**
3. Push dan otomatis deploy!

### Cara 2: Manual via gh-pages branch

1. Push ke GitHub (sama seperti di atas)
2. Di GitHub → Settings → Pages → Source: pilih branch `main`, folder `/ (root)`
3. Tunggu beberapa menit, site akan live!

## 📲 Install di HP

1. Buka link GitHub Pages di browser HP
2. **Android (Chrome):** Ketuk menu ⋮ → "Add to Home Screen"
3. **iPhone (Safari):** Ketuk share ↑ → "Add to Home Screen"

## 🛠️ Development

Cukup buka `index.html` di browser. Tidak perlu build tools atau server.

```bash
# Atau pakai live server:
python3 -m http.server 8000
# Buka http://localhost:8000
```

## 📁 Struktur File

```
workout-plan/
├── index.html      # Halaman utama (single-file app)
├── manifest.json   # PWA manifest
├── sw.js           # Service Worker untuk offline
├── icon-192.png    # Icon PWA 192x192
├── icon-512.png    # Icon PWA 512x512
└── README.md       # Dokumentasi
```

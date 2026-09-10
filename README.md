# IEEE OMÜ Computer Society — 2025–2026 Term Portfolio

Bu repository, **IEEE Ondokuz Mayıs Üniversitesi (OMÜ) Computer Society** komitesinin 2025–2026 çalışma dönemi boyunca gerçekleştirdiği etkinlikleri, teknik atölyeleri, projeleri ve topluluk faaliyetlerini sergilemek amacıyla hazırlanmış resmi portfolyo web sitesinin kaynak kodlarını içerir.

🌐 **Canlı Site:** [https://beyza-ozben.github.io/](https://beyza-ozben.github.io/)

---

## 🛠️ Kullanılan Teknolojiler

* **Framework:** [Astro v5](https://astro.build/) — Hızlı, içerik odaklı ve modern statik site mimarisi
* **Stil:** [Tailwind CSS](https://tailwindcss.com/) — Hızlı ve esnek arayüz tasarımı
* **Dağıtım (CI/CD):** [GitHub Actions](https://github.com/features/actions) & [GitHub Pages](https://pages.github.com/) — Otomatik derleme ve yayınlama boru hattı
* **Analitik:** [Google Analytics 4 (GA4)](https://analytics.google.com/) — Ziyaretçi trafiği ve etkileşim ölçümü

---

## 🚀 Yerel Geliştirme (Local Setup)

Projeyi kendi yerel ortamınızda çalıştırmak için aşağıdaki adımları izleyin:

### Gereksinimler
* **Node.js:** `v20.0.0` veya üzeri (Önerilen: `v22+`)
* **npm:** `v10+`

### Kurulum

1. Depoyu klonlayın:
```bash
git clone [https://github.com/beyza-ozben/beyza-ozben.github.io.git](https://github.com/beyza-ozben/beyza-ozben.github.io.git)
cd beyza-ozben.github.io
```

2. Bağımlılıkları yükleyin:
```bash
npm install
```

3. Geliştirme sunucusunu başlatın:
```bash
npm run dev
```
Tarayıcınızda `http://localhost:4321` adresine giderek siteyi inceleyebilirsiniz.

---

## 📦 Dağıtım (Deployment)

Bu repo, ana dala (`main`) yapılan her `push` işleminde otomatik olarak derlenen ve yayınlanan bir GitHub Actions iş akışına (`.github/workflows/deploy.yml`) sahiptir:

```bash
# Değişiklikleri ekleme ve gönderme
git add .
git commit -m "feat: site guncellemesi"
git push origin main
```

İş akışı adımları:
1. `main` dalına push yapıldığında GitHub Actions tetiklenir.
2. Proje Node.js ortamında otomatik derlenir (`npm run build`).
3. Oluşan `./dist` çıktısı GitHub Pages sunucularına aktarılır.

---

## 📂 Proje Dizini

```text
├── .github/workflows/   # CI/CD dağıtım yapılandırması
├── public/              # Statik dosyalar, görseller ve ikonlar
├── src/
│   ├── components/      # Tekrar kullanılabilir UI bileşenleri
│   ├── layouts/         # Sayfa düzenleri ve GA4 izleme betiği
│   └── pages/           # Site rotaları ve sayfalar
├── astro.config.mjs     # Astro yapılandırma ayarları
├── tailwind.config.mjs  # Tailwind CSS tema yapılandırması
└── package.json         # Proje bağımlılıkları ve betikleri
```

---

## 👤 İletişim & Geliştirici

* **Geliştirici:** Beyza Özben
* **GitHub:** [@beyza-ozben](https://github.com/beyza-ozben)
* **Topluluk:** [IEEE OMÜ Student Branch](https://www.ieeeomu.com/)
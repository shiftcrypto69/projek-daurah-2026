# 🛠️ Projek Daurah 2026: SVG Asset Extraction

Projek ini merupakan satu eksperimen teknikal dalam melakukan **Reverse Engineering** terhadap fail SVG yang kompleks (hasil eksport dari Canva) untuk dijadikan sebuah laman web statik yang ringan, responsif, dan mesra SEO.

## 🚀 Objektif Teknikal

1.  **Extraction**: Memisahkan data Base64 (imej binari) daripada struktur XML fail SVG.
2.  **Optimization**: Mengurangkan saiz fail asal (438KB) kepada struktur vektor bersih (0.74KB) dan aset imej JPEG yang dioptimumkan.
3.  **Hybrid Deployment**: Menggabungkan imej hasil ekstraksi dengan lapisan metadata HTML/CSS untuk keterlihatan enjin carian (SEO).

## 🛠️ Alatan & Teknologi

* **Python 3.14.2**: Digunakan untuk skrip ekstraksi `extract_svg_assets.py` dan pembersihan `clean_svg.py`.
* **HTML5 & CSS3**: Untuk membina *canvas* responsif dan lapisan teks (overlay).
* **GitHub Actions**: Automasi deployment ke GitHub Pages.
* **JSON-LD**: Metadata skema acara untuk pengindeksan Google yang lebih tepat.

## 📂 Struktur Projek

```text
├── .github/workflows/  # Automasi Deployment
├── images/             # Aset imej hasil extraction (poster_bg.jpg)
├── extract_svg_assets.py # Skrip Python Extraction
├── clean_svg.py        # Skrip Python Cleaning
├── index.html          # Struktur web & Metadata
└── style.css           # Seni bina visual responsif

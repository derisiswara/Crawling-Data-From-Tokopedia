# Crawling Data from Tokopedia

Proyek ini bertujuan untuk melakukan **web scraping** atau **crawling data** dari situs e-commerce **Tokopedia** untuk mengumpulkan informasi produk secara otomatis. Data yang diambil termasuk **nama produk**, **harga**, **rating**, **jumlah ulasan**, dan informasi lainnya yang berguna untuk keperluan riset atau analisis lebih lanjut.

## Fitur

- **Mengambil Data Produk**: Melakukan scraping pada halaman-halaman produk di Tokopedia dan mengambil data seperti nama produk, harga, rating, dan ulasan.
- **Penyimpanan Data**: Menyimpan hasil crawling dalam format **CSV** yang dapat digunakan untuk analisis lebih lanjut.
- **Mendukung Kategori Produk Berbeda**: Dapat melakukan crawling pada berbagai kategori produk di Tokopedia.
- **Headless Browsing**: Menggunakan **Selenium** untuk melakukan scraping secara otomatis tanpa memerlukan interaksi manual.

## Teknologi yang Digunakan

- **Python 3.x**: Bahasa pemrograman utama yang digunakan untuk proyek ini.
- **Selenium**: Digunakan untuk mengotomatisasi proses scraping, terutama untuk memuat halaman dinamis.
- **BeautifulSoup**: Untuk mengekstrak dan memparsing data HTML.
- **Requests**: Digunakan untuk mengirim permintaan HTTP ke halaman web yang ingin di-scrape.
- **Pandas**: Untuk manipulasi data dan menyimpan hasil scraping dalam format CSV.

## Struktur Proyek

```
|-- Main.ipynb
|-- README.md
|-- requirements.txt
```

## Cara Menjalankan Proyek

1. Clone repositori ini:

   ```bash
   git clone https://github.com/aqilwahid/Crawling-Data-From-Tokopedia.git
   ```

2. Install dependencies yang diperlukan:

   ```bash
   pip install -r requirements.txt
   ```

3. Pastikan Anda telah mengunduh dan mengkonfigurasi **WebDriver** untuk **Selenium** (misalnya, ChromeDriver untuk Google Chrome). Pastikan WebDriver ada di PATH Anda atau disimpan di lokasi yang diketahui.

4. Jalankan script utama untuk memulai proses crawling:

   ```bash
   python src/tokopedia_scraper.py
   ```

   Anda dapat menyesuaikan URL dan kategori produk yang ingin diambil dengan mengedit parameter di script.

5. Setelah proses crawling selesai, data yang terkumpul akan disimpan di folder `dataset/` dalam format CSV.

## Prasyarat

- **Python 3.x** harus sudah terinstall di sistem Anda.
- Install **WebDriver** yang sesuai dengan browser yang digunakan untuk Selenium (misalnya, **ChromeDriver** untuk Google Chrome).
- Pastikan koneksi internet yang stabil karena scraping memerlukan akses langsung ke halaman web.

## Catatan Penting

- Beberapa situs web termasuk Tokopedia mungkin memiliki aturan atau batasan mengenai scraping atau crawling data dari halaman mereka. Pastikan untuk mematuhi **robots.txt** dan kebijakan penggunaan mereka.
- Web scraping bisa memakan waktu tergantung pada jumlah data dan kecepatan pemuatan halaman.

## Kontribusi

Jika Anda memiliki ide atau perbaikan untuk proyek ini, jangan ragu untuk melakukan **fork** repositori, membuat branch baru, dan mengirim **pull request**.

1. Fork repositori ini.
2. Buat branch baru dengan fitur atau perubahan Anda.
3. Lakukan commit pada perubahan Anda.
4. Push branch Anda.
5. Buat pull request dan jelaskan perubahan yang Anda buat.

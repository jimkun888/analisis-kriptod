# Crypto Analyzer (versi desktop)

Aplikasi desktop (Electron) untuk memantau harga kripto, menganalisis koin, dan melihat prediksi harga.
Sumber data: CoinGecko (harga, market cap, riwayat harga), alternative.me (Fear & Greed), CryptoCompare (berita). Tanpa API key.

## Membuat file .exe di Windows
1. Pasang Node.js LTS dari https://nodejs.org (versi 18 atau lebih baru).
2. Ekstrak folder ini, buka Command Prompt di dalamnya.
3. Jalankan `npm install` (butuh internet, sekali saja).
4. Coba dulu dengan `npm start`.
5. Buat .exe dengan `npm run dist`. Hasilnya ada di folder `dist` (file portable `.exe`, tidak perlu instalasi).

## Catatan
- Pembaruan otomatis: harga tiap 30 detik, data penuh (Top 100, teknikal, berita, Fear & Greed) tiap 2 menit. Tombol Refresh tersedia untuk pembaruan manual.
- API gratis CoinGecko punya batas permintaan. Jika muncul "HTTP 429", tunggu semenit lalu klik Refresh.
- Data ETF tidak tersedia di versi ini. Perubahan harga 30 menit, 4 jam, dan 12 jam juga tidak tersedia.
- Indikator teknikal (SMA, RSI, MACD, Fibonacci, pivot) dihitung dari harga penutupan harian 365 hari; pivot adalah perkiraan sederhana.
- Daftar Berita, XAU/USD, dan USD/IDR di tab Beranda/Favorit/Berita masih snapshot tanggal 23-24 Nov 2026.
- Prediksi adalah model heuristik, bukan jaminan dan bukan nasihat keuangan.

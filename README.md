# Tebak Kata – Wordle Indonesia

Game tebak kata 5 huruf berbahasa Indonesia yang terinspirasi dari Wordle. Berjalan langsung di browser: satu file HTML, tanpa instalasi, tanpa dependensi.

## Cara bermain

Tebak kata rahasia 5 huruf dalam 6 kesempatan. Setelah setiap tebakan, warna petak memberi petunjuk:

- **Hijau**: huruf dan posisinya tepat.
- **Kuning**: huruf ada di kata rahasia, tetapi posisinya salah.
- **Abu-abu**: huruf tidak ada di kata rahasia.

Huruf ganda dihitung sesuai jumlah kemunculannya di kata rahasia.

## Fitur

- Sekitar 210 kata Indonesia sehari-hari, dipilih acak setiap permainan
- Keyboard layar dan keyboard fisik (huruf, Enter, Backspace)
- Warna pada keyboard layar ikut diperbarui sesuai hasil tebakan
- Animasi membalik petak dan getar saat huruf kurang
- Mode terang dan gelap otomatis mengikuti pengaturan perangkat
- Tampilan responsif untuk HP dan laptop
- Menghormati pengaturan `prefers-reduced-motion`

## Menjalankan

1. Unduh atau clone repositori ini:

   ```bash
   git clone https://github.com/USERNAME/NAMA-REPO.git
   cd NAMA-REPO
   ```

2. Buka file `index.html` di browser (klik dua kali).

Font Bricolage Grotesque dimuat dari Google Fonts. Jika tidak ada koneksi internet, game tetap berjalan dengan font bawaan sistem.

## Deploy ke GitHub Pages

1. Pastikan file utamanya bernama `index.html`.
2. Buka **Settings → Pages** di repositori.
3. Pada **Build and deployment**, pilih **Deploy from a branch**, lalu pilih branch `main` dan folder `/ (root)`.
4. Simpan. Game akan tersedia di `https://USERNAME.github.io/NAMA-REPO/`.

## Kustomisasi

Semua pengaturan ada di bagian `<script>` pada `index.html`:

- **Daftar kata**: edit konstanta `WORDS`. Tulis dengan huruf kecil a–z dan pisahkan dengan spasi. Kata yang panjangnya bukan 5 huruf otomatis diabaikan.
- **Jumlah kesempatan**: ubah nilai `MAX` (bawaan 6).
- **Warna**: ubah variabel CSS di `:root` (`--ok`, `--pres`, `--abs`).

## Catatan

- Tebakan tidak dicek ke kamus. Kamu bisa memasukkan huruf apa saja asalkan berjumlah 5.
- Daftar kata berisi kata umum dan tidak mengacu penuh pada KBBI.

## Teknologi

HTML, CSS, dan JavaScript murni (vanilla).

## Pembuat

Hossain Wismaya Rayhan

Emas Monitor v2 — Perbaikan 29 Okt 2026

Perbaikan:
- tidak memuat data demo TEGUH MAS
- tidak menggunakan cache data lama saat API gagal
- query membaca view gold_price_dashboard yang sekarang memiliki store_name_y dan store_name_y_dummy (tanpa store_name)
- label toko lain diturunkan dari data aktual; jika toko tidak ada di view maka tidak muncul di legend
- harga buyback per gram dikonversi per keping untuk spread
- tanpa perubahan SQL atau data Supabase

Deploy ke Vercel (project yang sama):
- Ekstrak ZIP ke folder lokal.
- Gunakan Vercel CLI dari folder tersebut: npx vercel link (pilih existing project), lalu npx vercel --prod.
- Atau commit file ke repo GitHub yang terhubung ke project Vercel untuk deployment otomatis.
- Vercel Drop biasanya membuat project terpisah, jadi jangan gunakan Drop jika mau mempertahankan URL lama.

Koneksi:
- Buka halaman baru; klik Settings.
- Isi URL project (sudah dipraisi Family) dan publishable key Supabase, BUKAN secret/service_role key.
- Key tersimpan di browser normal, tidak ikut ke Incognito.
- Jika view error, layar akan menampilkan pesan kesalahan dan grafik kosong, bukan simulasi.

Tidak ada data dummy dalam ZIP ini.

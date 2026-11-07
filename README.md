# Ajak Nongkrong (stack gratis)

Supabase (database, login, realtime) + hosting statis gratis.

1. Buat proyek di supabase.com (paket Free).
2. SQL Editor: tempel dan jalankan `supabase/schema.sql`.
3. Login memakai tautan email bawaan Supabase, jadi template tidak perlu diubah. (Template baru bisa diedit setelah memasang SMTP sendiri.)
4. Settings > API: salin Project URL dan anon key ke bagian atas `index.html` (`SB_URL`, `SB_KEY`). Anon key aman dipakai di browser karena data dilindungi RLS.
5. Hosting gratis: unggah folder ini ke Cloudflare Pages, Netlify, atau GitHub Pages. Tambahkan alamat situs di Authentication > URL Configuration.

Batasan paket gratis dan yang belum ada:
- Proyek Free dijeda jika seminggu tanpa aktivitas. Kuota email bawaan sangat kecil, jadi pasang SMTP gratis (mis. Brevo atau Resend) sebelum dipakai banyak orang.
- Verifikasi selfie otomatis tidak ada yang gratis. Sementara, tinjau manual lalu ubah kolom `verified` di Table Editor.
- Belum ada pembatasan laju (rate limit) untuk pencarian lokasi. Tambahkan sebelum dibuka untuk umum, dan tinjau tabel `reports` secara rutin.
- Lencana pertemuan, bagikan rencana ke kontak darurat, dan radar belum ada di versi ini.

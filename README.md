# airasia24jam.id

Panduan informasi independen reschedule AirAsia. Bukan situs resmi AirAsia.

## GitHub → Cloudflare Workers (Static Assets)

Upload **isi folder paket** ke root repository `rescheduleairasia/airasia` dengan mempertahankan folder `public` dan `img`. Jangan upload ZIP tanpa ekstrak.

Cloudflare Workers Builds: repository `rescheduleairasia/airasia`, branch `main`, build command kosong, deploy command `npx wrangler deploy`. Tidak diperlukan worker.js. Setelah deploy berhasil, hubungkan custom domain airasia24jam.id.

Jika error `assets.directory does not exist`, periksa bahwa `public/index.html` benar-benar ada pada root repository (bukan di folder tambahan).

# Yukki Music Bot Configs

Config vars pada dasarnya adalah variabel yang mengonfigurasi atau memodifikasi bot agar berfungsi, yang merupakan kebutuhan dasar plugin atau kode agar berfungsi. Anda harus mengatur vars wajib yang tepat untuk membuatnya berfungsi

- Ini adalah vars minimum yang diperlukan untuk membuat Yukki Music Bot berfungsi.

1. `API_ID` : Dapatkan dari my.telegram.org
2. `API_HASH` : Dapatkan dari my.telegram.org 
3. `BOT_TOKEN` : Get it from [@Botfather](http://t.me/BotFather) in Telegram
4. `MONGO_DB_URI` : dapatkan mongo db [disini](https://www.mongodb.com)
5. `LOG_GROUP_ID` ​​: Buatlah Group Super /public group dan masukan bot Rose ketik /id
7. `OWNER_ID` : ID Pemilik Anda untuk mengelola bot Anda.
8. `STRING_SESSION` : Diperlukan Sesi Pyrogram, Hasilkan string dari [@xastringbot](http://t.me/xastringbot) di Telegram.


## Vars Tidak Wajib

- Ini adalah vars tambahan untuk fitur tambahan di dalam Bot Musik. Anda dapat meninggalkan vars yang tidak wajib untuk saat ini dan dapat menambahkannya nanti.

1. `DURATION_LIMIT` : Durasi audio (musik) maks khusus untuk obrolan suara. Default untuk 60 menit.
2. `SONG_DOWNLOAD_DURATION_LIMIT` : Batas Durasi untuk mendownload Lagu dalam format MP3 atau MP4 dari bot. Default ke 180 menit.
3. `VIDEO_STREAM_LIMIT` : Jumlah maksimum panggilan video yang diizinkan di bot. Nanti bisa diatur lewat /set_video_limit di telegram. Default untuk 3 obrolan.
4.`SERVER_PLAYLIST_LIMIT`: Batas Maksimum Diizinkan bagi pengguna untuk menyimpan daftar putar di server bot. Standar ke 30
6. `CLEANMODE_MINS` : Waktu Cleanmode setelah bot akan menghapus pesan lama dari obrolan. Default ke 5 Menit.
7. `SUPPORT_CHANNEL` : Jika Anda memiliki saluran untuk bot musik Anda, isi dengan tautan saluran Anda
8. `SUPPORT_GROUP` : Jika Anda memiliki dukungan grup untuk bot musik Anda, isi dengan tautan saluran Andae Limit Vars

## Putar Batas Ukuran File Vars

- Batas ukuran file maksimum untuk audio dan video yang dapat diputar pengguna dari bot Anda. [Hanya Ukuran Byte yang Diterima]
> Anda dapat mengonversi mb menjadi byte dari https://www.gbmb.org/mb-to-bytes dan menggunakannya di sini

1. `TG_AUDIO_FILESIZE_LIMIT` : Batas ukuran file maksimum untuk file audio yang dapat dialirkan melalui vc. Default ke 104857600 byte, yaitu 100MB
2. `TG_VIDEO_FILESIZE_LIMIT` : Batas maksimum ukuran file untuk file video yang dapat diputar. Default ke 1073741824 byte, yaitu 1024MB atau 1GB

## Bot Vars

- Ini semua vars digunakan untuk mengatur bot. Anda dapat mengedit vars ini jika Anda mau, jika tidak, biarkan semuanya apa adanya.

1. `PRIVATE_BOT_MODE` : Setel true jika Anda ingin bot Anda menjadi pribadi saja atau False untuk semua grup. Default ke Salah
2. `YOUTUBE_EDIT_SLEEP` : Durasi waktu tidur Untuk Youtube Downloader. Default ke 3 detik
3. `TELEGRAM_EDIT_SLEEP` : Durasi waktu tidur Untuk Telegram Downloader. Default ke 5 detik
4. `AUTO_LEAVING_ASSISTANT` : Setel ke True jika Anda ingin meninggalkan asisten setelah jangka waktu tertentu.
5. `ASSISTANT_LEAVE_TIME` : Waktu setelah akun asisten Anda akan meninggalkan obrolan yang dilayani secara otomatis. Default ke 5400 detik, yaitu 90 Menit
6. `AUTO_DOWNLOADS_CLEAR` : Setel True jika Anda ingin menghapus unduhan setelah pemutaran musik berakhir.
7. `AUTO_SUGGESTION_MODE` : Setel True jika Anda ingin bot menyarankan tentang perintah bot ke obrolan acak bot Anda.
9. `AUTO_SUGGESTION_TIME` : Waktu setelah bot Anda akan menyarankan 1/10 obrolan acak dari obrolan yang Anda layani tentang perintah bot. Default ke 5400 detik, yaitu 90 Menit

## Spotify Vars

- Anda dapat memutar trek atau daftar putar dari spotify dari bot Yukki Music
- Anda akan membutuhkan dua vars ini untuk membuat permainan spotify berfungsi. Ini tidak penting, Anda dapat membiarkannya kosong jika Anda mau.

1. `SPOTIFY_CLIENT_ID` : Dapatkan dari https://developer.spotify.com/dashboard
2. `SPOTIFY_CLIENT_SECRET` : Dapatkan dari https://developer.spotify.com/dashboard

## Heroku Vars

- Untuk menjalankan beberapa modul yang kompatibel dengan Heroku, nilai var ini diperlukan untuk Mengakses akun Anda untuk menggunakan perintah `get_log`, `usage`, `update` dll dll.
- Anda dapat mengisi var ini menggunakan kunci API atau token Otorisasi Anda.

1. `HEROKU_API_KEY` : Dapatkan dari http://dashboard.heroku.com/account
2. `HEROKU_APP_NAME` : Anda harus memasukkan nama aplikasi yang Anda berikan untuk mengidentifikasi Bot Musik Anda di Heroku.

## Kustom Repo Vars

- Jika Anda berencana untuk menggunakan Yukki Music Bot dengan kode Anda sendiri yang disesuaikan atau dimodifikasi.

1. `UPSTREAM_REPO` : URL Repo Upstream Anda atau Repo Bercabang.
2. `UPSTREAM_BRANCH` : Cabang Default dari URL Repo Hulu atau Repo Bercabang Anda.
3. `GIT_TOKEN` : GIT TOKEN Anda jika repo upstream Anda bersifat pribadi
4. `GITHUB_REPO` : URL Repo Github Anda, yang akan ditampilkan pada perintah /start

## Gambar/Thumbnail Vars

- Anda dapat mengubah gambar yang digunakan di Yukki Music Bot.
- Anda dapat membuat tautan telegaph dari [@YukkiTelegraphBot](http://t.me/YukkiTelegraphBot) dan menggunakannya di sini.

1. `START_IMG_URL` : Gambar yang muncul pada perintah /start dalam pesan pribadi bot.
2. `PING_IMG_URL` : Gambar yang muncul pada perintah /ping bot.
3. `PLAYLIST_IMG_URL` : Gambar yang muncul pada perintah /play bot.
4. `GLOBAL_IMG_URL` : Gambar yang muncul pada perintah /stats bot.
5. `STATS_IMG_URL` : Gambar yang muncul pada perintah /stats bot.
6. `TELEGRAM_AUDIO_URL` : Gambar ini muncul ketika seseorang memutar audio dari telegram.
7. `TELEGRAM_VIDEO_URL` : Gambar ini muncul saat seseorang memutar video dari telegram.
8. `STREAM_IMG_URL` : gambarnya muncul ketika seseorang memainkan m3u8 atau tautan indeks.
9. `SOUNCLOUD_IMG_URL` : Gambar ini muncul saat seseorang memutar musik dari soundcloud.
10. `YOUTUBE_IMG_URL` : Gambar ini muncul jika pembuat thumbnail gagal untuk membuat ibu jari.
11. `SPOTIFY_ARTIST_IMG_URL` : Gambar ini muncul saat seseorang memutar artis Spotify melalui tautan dalam mode sebaris.
12. `SPOTIFY_ALBUM_IMG_URL` : Gambar ini muncul ketika seseorang memutar album Spotify melalui tautan dalam mode sebaris.
13. `SPOTIFY_PLAYLIST_IMG_URL` : Gambar ini muncul ketika seseorang memutar album Spotify melalui tautan dalam mode sebaris.

## Multi Assistant Mode

- Anda dapat menggunakan hingga 5 Asisten Klien (memungkinkan bot Anda setidaknya bekerja dalam 2000-2500 obrolan sekaligus)

1. `STRING_SESSION2` : Diperlukan Sesi Pyrogram, Hasilkan string dari [@xastringbot](http://t.me/xastringrobot) di Telegram.
2. `STRING_SESSION3` : Diperlukan Sesi Pyrogram, Hasilkan string dari [@xastringbot](http://t.me/xastringrobot) di Telegram.
3. `STRING_SESSION4` : Diperlukan Sesi Pyrogram, Hasilkan string dari [@xastringbot](http://t.me/xastringrobot) di Telegram.
4. `STRING_SESSION5` : Diperlukan Sesi Pyrogram, Hasilkan string dari [@xastringbot](http://t.me/xastringbot) di Telegram.

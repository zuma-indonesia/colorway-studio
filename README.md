# Sandal Colorway Studio

Web untuk mencoba kombinasi warna sandal per model (filter Gender → Series).

## Login & akses

Login pakai akun Google @zuma.id. Foto dibaca **langsung dari Google Drive** memakai akun yang login,
jadi yang bisa melihat sandal = akun yang punya akses ke folder Drive **Colorway Studio**
(Shared Drive " Zuma Reports"). Tambah orang = share folder Drive-nya. Repo ini hanya berisi kode, tanpa foto.

`CLIENT_ID` di `index.html` = OAuth Client ID (Web application) dari Google Cloud, consent screen *Internal* (zuma.id),
scope `drive.readonly`. Authorized JavaScript origins: `https://zuma-indonesia.github.io`, `http://localhost:8090`.

## Menambah / mengganti model

```
Colorway Studio / <Gender> / <Series> / 1 sole.png, 2 upper.png, 3 logo.png, ...
```

- Nomor = urutan tumpukan (1 = paling bawah); teks sesudah nomor = nama bagian di web.
- Semua PNG transparan, ukuran sama persis, posisi tidak bergeser.
- Nama bagian mengandung `stripe`/`garis`/`list` diwarnai polos (tanpa shading).
- Foto yang salah nama muncul sebagai peringatan kuning di web; salah ukuran muncul saat model dipilih.

## Jalan di lokal

```
python3 -m http.server 8090      # buka http://localhost:8090
```

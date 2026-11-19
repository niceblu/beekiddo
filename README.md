# BeeKIDDO — versi GitHub Pages

Isi folder ini adalah tampilan (front end) BeeKIDDO. Datanya tetap disimpan di Google Apps Script + Google Sheets milik Anda.

## File
- `index.html` — seluruh aplikasi (satu file)
- `config.js` — alamat Apps Script (`BK_API_URL`). Ubah di sini bila Anda membuat deployment baru.
- `.nojekyll` — agar GitHub Pages menyajikan file apa adanya

## Langkah deploy
1. **Apps Script**: ganti isi `Code.gs`, `DefaultData.gs` dengan versi baru (Index/Script/Styles/Assets boleh tetap ada, tidak dipakai GitHub). Jalankan `setup()` sekali bila diminta.
2. **Deploy ulang**: Deploy ▸ Manage deployments ▸ ✏️ ▸ Version: *New version* ▸ Deploy. URL `/exec` tetap sama. Pastikan *Execute as: Me* dan *Who has access: Anyone*.
3. **Cek**: buka `…/exec?api=ping` di browser, harus muncul `{"ok":true,...}`.
4. **GitHub**: buat repo, unggah isi folder ini ke root, lalu Settings ▸ Pages ▸ Deploy from a branch ▸ `main` / root.
5. **Alamat situs**: buka aplikasi ▸ ketuk logo 5× ▸ PIN admin ▸ tab Permintaan ▸ isi *Alamat situs* dengan URL GitHub Pages Anda ▸ Simpan (supaya tautan di email mengarah ke sana).
6. Ganti PIN admin bawaan (1234).

# geo_catatan
## Nama : inandiar sharfina fauzi
## NIM : 362458302078
## prodi : Teknologi rekayasa perangkat lunak

## TugasMandiri
 1. Kustomisasi Marker:Ubah ikon marker agar berbeda-beda tergantung jenis catatan(misal:Toko,Rumah,Kantor). 

kode yang di tambahankan:

  <img width="1738" height="1496" alt="image" src="https://github.com/user-attachments/assets/600d16fe-f607-4944-ab02-448d9fa72596" />

 <img width="1552" height="1422" alt="image" src="https://github.com/user-attachments/assets/4c5e833e-bc02-4a61-9d1a-a08e4b9955d1" />
 PENJELASAN:
 Digunakan untuk membedakan marker pada peta dengan cara menetapkan ikon dan warna yang unik, yang ditentukan oleh jenis catatan yang disimpan (seperti 'Toko', 'Kantor', atau 'Rumah'). Proses kustomisasi ini dikendalikan oleh dua fungsi helper: _getIconForType yang memilih simbol (IconData) yang sesuai, dan _getColorForType yang menentukan skema warna. Kedua nilai ini kemudian diterapkan pada setiap objek Marker saat data _savedNotes diproses. Hal ini memastikan bahwa ikon dan warna marker selalu sinkron dengan properti n.jenis data, sehingga meningkatkan kemudahan pengguna dalam mengidentifikasi dan membedakan kategori lokasi di peta secara visual.
 
 
2.  HapusData : Tambahkan fitur untuk menghapus marker yang sudah dibuat.
    
 kode: 
 <img width="1720" height="1236" alt="image" src="https://github.com/user-attachments/assets/29b5b979-daef-40f5-b8c3-4b30f7dc3663" />
 
 PENJELASAN :
 fungsi _showDeleteDialog merupakan mekanisme konfirmasi dan eksekusi penghapusan marker. Fungsi ini menampilkan dialog untuk mendapatkan persetujuan pengguna, dan jika dikonfirmasi, ia akan menghapus objek catatan dari data (_savedNotes.remove(note)) dan memperbarui penyimpanan (_saveNotes()), memastikan marker tersebut hilang secara permanen dari peta dan aplikasi.
 

 3. Simpan Data (Opsional) Gunakan SharedPreferences atau Hive agar data tidak hilang saat aplikasi ditutup
    
 kode: 
 
 <img width="1350" height="1422" alt="image" src="https://github.com/user-attachments/assets/b36572ed-a559-4b79-a5fa-3d8d9557f23b" />
 PENJELASAN :
 Fungsi _saveNotes() melakukan serialisasi data catatan menjadi JSON String untuk disimpan ke disk, sementara _loadNotes() menangani deserialisasi (memuat dan mengembalikan data) saat aplikasi dimulai melalui initState(), yang secara  bersatu menjamin data marker tersimpan dan dimuat kembali secara otomatis tanpa hilang.
##  HASILNYA:

- tampilan awal
  
  
![WhatsApp Image 2025-11-21 at 21 07 59_5f6d4eda](https://github.com/user-attachments/assets/be803d50-b21e-43af-84df-9fe36a3e4a4b)

- menambahkan catatan
  
![WhatsApp Image 2025-11-21 at 21 10 21_cb3f74d4](https://github.com/user-attachments/assets/50ec9c1e-391d-494c-9664-3e9fb0547a33)

- tampilan catatan yang telah di buat
  
![WhatsApp Image 2025-11-21 at 21 22 24_ba94f364](https://github.com/user-attachments/assets/de83c313-9213-4337-b71d-7b7d7fad85bc)

- Hapus catatan
  
![WhatsApp Image 2025-11-21 at 21 08 01_24d08d51](https://github.com/user-attachments/assets/13ef56f0-155c-476d-b30c-59d496de8bdf)

- setelah di hapus catatannya
  
![WhatsApp Image 2025-11-21 at 22 26 56_73b6490e](https://github.com/user-attachments/assets/73d6e2c2-f822-4806-81fe-34bc73d8cbea)





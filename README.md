# Pertemuan 11 Dictionary/Map
Nama: Eka Elsanti
NIM: 2225250059
Kelas: 3A

## Tujuan
Memodelkan data pendidikan menggunakan dictionary dan pasangan key-value.

## Struktur Data
- **Key Utama:** NIM (String) sebagai identitas unik.
- **Value:** Dictionary bertingkat yang menyimpan nama (`string`), kelas (`string`), dan nilai (`integer`).

## Cara Menjalankan
```bash
python3 praktik/data_mahasiswa.py

```

## Test Case

| Kasus | Input/Aksi | Hasil yang Diharapkan | Hasil Aktual | Status |
| --- | --- | --- | --- | --- |
| Pencarian tersedia | A003 | Data Citra ditampilkan | Data Citra ditampilkan | Lulus |
| Pencarian tidak tersedia | A999 | Pesan 'Data tidak ditemukan' | Pesan 'Data tidak ditemukan' | Lulus |
| Pembaruan nilai | A002 menjadi 82 | Nilai A002 berubah menjadi 82 | Nilai A002 berubah menjadi 82 | Lulus |
| Penambahan data | A006 | Key A006 tersedia | Key A006 tersedia | Lulus |
| Rekap | items() | Semua NIM dan data tampil | Semua NIM dan data tampil | Lulus |

## Refleksi

Penggunaan kurung siku `data['key']` pada key yang tidak ada akan memicu `KeyError`. Masalah ini diatasi menggunakan method `.get('key')` yang mengembalikan `None` atau pesan default secara aman.
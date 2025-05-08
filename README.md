# SAFPSUnlock
# FPSUnlock.ASI untuk GTA San Andreas

## Deskripsi
Plugin ASI ini menghilangkan batasan 30 FPS di Grand Theft Auto: San Andreas (versi 1.0 US), memungkinkan game berjalan pada frame rate yang lebih tinggi untuk gameplay yang lebih halus. Termasuk penyesuaian fisika untuk menjaga stabilitas game pada FPS tinggi.

## Fitur
- Menghilangkan batas 30 FPS (tidak terbatas atau bisa disesuaikan)
- Penyesuaian skala waktu fisika
- Konfigurasi melalui file INI
- Kompatibel dengan CLEO dan mod ASI lainnya
- Bekerja untuk versi 32-bit dan 64-bit

## Cara Instalasi
1. Salin file berikut ke folder utama GTA SA (tempat gta_sa.exe berada):
   - `FPSUnlock.asi`
   - `FPSUnlock.ini`
   - (Opsional) `MinHook.x64.dll` jika tidak terlink secara statis

2. Pastikan Anda memiliki:
   - ASI Loader (disarankan [Ultimate ASI Loader](https://github.com/ThirteenAG/Ultimate-ASI-Loader))
   - Versi GTA SA v1.0 US

## Konfigurasi
Edit `FPSUnlock.ini` untuk menyesuaikan pengaturan:
```ini
[Settings]
UnlockFPS = true       ; Set false untuk menonaktifkan
CustomFPS = 0          ; 0 untuk tidak terbatas, atau atur FPS yang diinginkan (contoh: 60, 144)
PhysicsScale = 1.0     ; jangan dirubah
```

## Pengaturan yang Disarankan
| Refresh Rate Monitor | CustomFPS yang Disarankan | PhysicsScale |
|----------------------|---------------------------|--------------|
| 60Hz                 | 60                        | 1.0          |
| 75Hz                 | 75                        | 0.9          |
| 120Hz                | 120                       | 0.7          |
| 144Hz                | 144                       | 0.6          |
| 240Hz+               | 0 (tidak terbatas)        | 0.5          |

## Pemecahan Masalah
**Game terlalu cepat:**
- Turunkan nilai `PhysicsScale`
- Setel batas `CustomFPS`

**Game crash:**
- Pastikan versi game 1.0 US
- Instal ASI Loader terbaru
- Coba jalankan sebagai administrator

**Masalah fisika:**
- Naikkan nilai `PhysicsScale`
- Batasi FPS sesuai refresh rate monitor

## Kredit
- MinHook oleh Tsuda Kageyu
- INIReader oleh Ben Hoyt
- Riset memori GTA SA oleh berbagai modder

## Penafian
Gunakan dengan risiko sendiri. Selalu backup save game sebelum memasang mod. Tidak bertanggung jawab atas ketidakstabilan game atau kerusakan save file.

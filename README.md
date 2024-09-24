# QR-Code-Face-Recognition-Door-Lock-System---Arduino-IoT
# Sistem Kunci Pintu QR Code dan Pengenalan Wajah - Arduino IoT

Proyek ini mendemonstrasikan sistem kunci pintu pintar yang menggabungkan teknologi pemindaian kode QR dan pengenalan wajah, dikendalikan oleh sistem IoT berbasis Arduino. Sistem ini meningkatkan keamanan dengan menggunakan dua metode autentikasi (kode QR dan pengenalan wajah) untuk mengontrol akses ke area yang aman.

## Daftar Isi
- [Gambaran Umum](#gambaran-umum)
- [Fitur](#fitur)
- [Komponen](#komponen)
- [Instalasi](#instalasi)
- [Penggunaan](#penggunaan)
- [Kontribusi](#kontribusi)
- [Lisensi](#lisensi)

## Gambaran Umum
Sistem ini menggunakan pemindai kode QR dan modul pengenalan wajah untuk mengautentikasi pengguna sebagai kontrol akses. Sistem ini dirancang untuk bekerja bersama dengan Arduino, yang terhubung ke berbagai modul seperti kamera dan sistem relay untuk operasi pintu. Ketika pengguna memindai kode QR yang valid dan wajahnya dikenali, pintu akan terbuka. Jika salah satu dari pemeriksaan ini gagal, akses akan ditolak.

## Fitur
- *Autentikasi Kode QR*: Memindai kode QR yang diberikan kepada pengguna untuk memverifikasi keabsahan.
- *Pengenalan Wajah*: Menggunakan kamera dan perangkat lunak pengenalan wajah untuk memverifikasi identitas pengguna.
- *Integrasi IoT*: Sistem ini dapat dikelola secara jarak jauh menggunakan protokol IoT untuk memantau dan mengontrol pintu.
- *Kendali Arduino*: Menggunakan papan Arduino untuk mengelola semua pemrosesan dan sinyal kontrol.
- *Autentikasi Dua Faktor*: Menggabungkan kode QR dan pengenalan wajah untuk keamanan yang tinggi.

## Komponen
Untuk membangun proyek ini, Anda memerlukan komponen berikut:
1. Arduino Uno atau mikrokontroler yang kompatibel
2. Modul Pemindai Kode QR
3. Modul Kamera untuk Pengenalan Wajah
4. Modul Relay (untuk mengendalikan kunci pintu)
5. Servo Motor (untuk mekanisme kunci/buka)
6. Modul Wi-Fi (ESP8266/ESP32) untuk integrasi IoT
7. Breadboard dan kabel penghubung
8. Catu daya untuk Arduino dan modul lainnya
9. Mekanisme kunci pintu elektronik

## Instalasi
### 1. Pengaturan Perangkat Keras
- Hubungkan pemindai kode QR dan modul kamera ke Arduino.
- Hubungkan relay ke Arduino untuk mengendalikan mekanisme kunci.
- Atur modul Wi-Fi untuk terhubung ke dashboard IoT Anda untuk pemantauan jarak jauh.
- Rangkaikan semua komponen sesuai dengan skema yang disediakan.

### 2. Pengaturan Perangkat Lunak
- Instal Arduino IDE jika belum terpasang. Anda dapat mengunduhnya dari [sini](https://www.arduino.cc/en/software).
- Instal library yang diperlukan untuk pemindaian kode QR, pengenalan wajah, dan integrasi IoT (misalnya, ESP8266WiFi, Servo, dll.).
- Unggah sketch Arduino dari repositori ini ke papan Arduino Anda.

### 3. Integrasi IoT
- Konfigurasikan platform IoT Anda (misalnya, Blynk, ThingsBoard) untuk memantau dan mengontrol sistem kunci pintu secara jarak jauh.
- Atur notifikasi dan log untuk melacak kejadian akses.

## Penggunaan
1. Pindai kode QR yang diberikan kepada pengguna.
2. Jika kode QR valid, sistem akan melanjutkan ke pengenalan wajah.
3. Kamera akan menangkap wajah pengguna dan memeriksanya dengan database yang tersimpan.
4. Jika kedua pemeriksaan (kode QR dan pengenalan wajah) berhasil, pintu akan terbuka.
5. Jika salah satu pemeriksaan gagal, akses akan ditolak.

## Pemecahan Masalah
- *Masalah: Kode QR tidak dikenali*  
  Solusi: Pastikan modul pemindai terhubung dengan benar dan menerima daya yang cukup. Periksa apakah kode QR jelas dan tidak rusak.
  
- *Masalah: Pengenalan wajah gagal*  
  Solusi: Sesuaikan kondisi pencahayaan atau pastikan kamera diposisikan dengan benar. Pastikan database wajah diperbarui dan akurat.

- *Masalah: Dashboard IoT tidak terhubung*  
  Solusi: Verifikasi bahwa kredensial Wi-Fi benar dan modul terhubung ke jaringan. Periksa pengaturan dashboard untuk pendaftaran perangkat yang benar.

## Kontribusi
Kontribusi sangat disambut! Jangan ragu untuk membuka issue atau mengirimkan pull request untuk meningkatkan fungsionalitas proyek ini.

## Lisensi
Proyek ini dilisensikan di bawah Lisensi MIT. Lihat file LICENSE untuk informasi lebih lanjut.

---

Template ini bisa kamu modifikasi sesuai kebutuhan dan struktur spesifik dari proyekmu.

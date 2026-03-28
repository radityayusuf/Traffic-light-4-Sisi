# Tugas 3 - Simulasi Traffic Light 4 Arah (Arduino Uno) 🚦

Repositori ini berisi *source code* dan dokumentasi untuk simulasi sistem kendali lampu lalu lintas 4 arah menggunakan mikrokontroler Arduino Uno. Proyek ini dikerjakan sebagai pemenuhan Tugas 3 mata kuliah **Pemrograman Sistem Tertanam (IF21605)**.

**Disusun oleh:**
* **Nama:** Raditya Yusuf Ramadhan
* **NIM:** H1D023056
* **Program Studi:** Informatika, Universitas Jenderal Soedirman
  
<img width="1085" height="718" alt="Screenshot 2026-03-28 195952" src="https://github.com/user-attachments/assets/e8a42373-2802-4d57-a159-2950bc720fe0" />


## 📝 Deskripsi Proyek
Sistem ini mensimulasikan persimpangan jalan dengan 4 arah (Utara, Timur, Selatan, Barat). Lampu hijau akan menyala secara bergantian memutar searah jarum jam. Sistem ini dirancang agar bekerja secara otomatis dan berulang (*looping*) dengan menerapkan konsep fungsi modularisasi untuk efisiensi kode.

**Aturan Waktu (Timing):**
1. **Lampu Hijau:** Menyala selama 5 detik.
2. **Lampu Kuning:** Memberikan efek berkedip cepat 3 kali, dilanjutkan menyala statis selama 2 detik.
3. **Lampu Merah:** Merupakan kondisi *default* (berhenti) untuk semua simpang yang sedang tidak aktif.
*Catatan: Sistem diatur agar tidak ada lebih dari satu simpang yang menyalakan lampu hijau secara bersamaan.*

---

## 🛠️ Komponen Hardware (Tinkercad)
Rangkaian fisik pada simulasi ini menggunakan komponen berikut:
* 1x Arduino Uno R3
* 1x Breadboard
* 12x LED (4 Merah, 4 Kuning, 4 Hijau)
* 12x Resistor 220 Ω
* Kabel Jumper secukupnya

---

## 🔌 Skema Pin (Wiring)
Semua kaki Katoda LED dihubungkan ke Ground (GND). Kaki Anoda dihubungkan ke pin digital Arduino melalui resistor 220 Ohm dengan konfigurasi berikut:

| Simpang | LED Merah | LED Kuning | LED Hijau |
| :--- | :---: | :---: | :---: |
| **Utara** | Pin 2 | Pin 3 | Pin 4 |
| **Timur** | Pin 5 | Pin 6 | Pin 7 |
| **Selatan**| Pin 8 | Pin 9 | Pin 10 |
| **Barat** | Pin 11 | Pin 12 | Pin 13 |

---

## 🚀 Tautan Simulasi
Kamu bisa melihat dan menjalankan simulasi rangkaian ini secara langsung di Tinkercad melalui tautan berikut:
👉 https://www.tinkercad.com/things/kUkptrcf2tr-traffic-light-4-arah?sharecode=undefined



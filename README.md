# Tugas Besar 1 Strategi Algoritma: MIT Battlecode Bot (GreedyPainter)

Repositori ini berisi implementasi kecerdasan buatan (AI) / Bot untuk permainan **MIT Battlecode**. Bot ini diberi nama **GreedyPainter** karena menggunakan pendekatan algoritma *Greedy* (Rakus) untuk mengambil keputusan optimal secara lokal di setiap *turn* (giliran).

Repositori ini ditulis 100% menggunakan bahasa **Java**.

## 📌 Deskripsi Strategi (Algoritma Greedy)
Bot ini mengontrol beberapa jenis unit robot dengan prinsip *greedy* sebagai berikut:
1. **Navigasi & Jarak:** Unit selalu memilih target (musuh, reruntuhan/ruin, atau menara kawan) yang posisinya paling dekat saat itu juga.
2. **Efisiensi Serangan (Splasher):** Selalu menyemburkan cat ke area yang memberikan skor tertinggi (paling banyak mengecat area kosong atau menimpa cat musuh).
3. **Sapuan Maksimal (Mopper):** Sebelum mengayunkan alat pembersih (*mop swing*), unit akan menghitung arah yang mengenai jumlah musuh paling banyak.
4. **Manajemen Sumber Daya:** Tower akan langsung memproduksi unit baru (dengan urutan tertentu) begitu sumber daya (chip dan cat) mencukupi, tanpa menabung.

## 🤖 Peran Unit Robot
- **Tower:** Bertahan, melakukan *upgrade*, dan memproduksi unit (Splasher, Mopper, Soldier).
- **Soldier:** Unit pekerja dan kombatan dasar; bertugas mencari reruntuhan (*ruins*) untuk membangun tower baru.
- **Splasher:** Unit spesialis area; bertugas mengecat peta secara masif dan efisien.
- **Mopper:** Unit jarak dekat; bertugas membersihkan cat musuh dan melakukan serangan sapuan (*mop swing*) ke gerombolan musuh.

## 🚀 Cara Menjalankan (How to Run)
Karena ini adalah proyek MIT Battlecode, pastikan Anda telah menginstal JDK yang sesuai.

1. *Clone* repositori ini:
   ```bash
   git clone https://github.com/LeonArif/Tubes1_STIma.git
   cd Tubes1_STIma
   ```
2. Jalankan *client* Battlecode menggunakan Gradle:
   ```bash
   # Di sistem operasi Windows:
   gradlew run

   # Di sistem operasi Mac/Linux:
   ./gradlew run
   ```
3. Pilih bot `GreedyPainter` pada antarmuka Battlecode untuk mempertandingkannya.

## 👥 Identitas Pembuat
* Tugas Besar 1 Mata Kuliah Strategi Algoritma (STIma)
* Dibuat oleh: **Leon Arif** (dan tim, jika ada)

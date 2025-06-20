Aplikasi Grafis 2D adalah sebuah aplikasi berbasis web yang memungkinkan pengguna untuk:

Menggambar berbagai bentuk geometri (titik, garis, persegi, ellipse)
Memilih dan memanipulasi objek yang telah digambar
Melakukan transformasi geometri (translasi, rotasi, scaling)
Mengelola daftar objek yang telah dibuat

✨ Fitur Utama
🖊️ Alat Gambar

Titik: Membuat titik dengan ukuran yang dapat disesuaikan
Garis: Menggambar garis lurus dengan drag and drop
Persegi: Membuat persegi panjang dengan drag and drop
Ellipse: Menggambar ellipse/lingkaran dengan drag and drop

🎨 Kustomisasi

Pemilihan Warna: Color picker untuk memilih warna objek
Ketebalan Garis: Slider untuk mengatur ketebalan garis (1-20 px)
Preview Real-time: Melihat bentuk objek saat menggambar

🔧 Transformasi Geometri

Translasi: Memindahkan objek ke posisi baru
Rotasi: Memutar objek dengan sudut tertentu
Scaling: Mengubah ukuran objek (memperbesar/memperkecil)
Transformasi Cepat: Tombol shortcut untuk transformasi umum

📋 Manajemen Objek

Daftar Objek: Melihat semua objek yang telah dibuat
Seleksi Objek: Memilih objek dengan klik
Hapus Objek: Menghapus objek terpilih atau semua objek
Visual Feedback: Highlighting objek yang dipilih

🚀 Cara Penggunaan
Memulai Aplikasi

Buka file HTML di browser web
Aplikasi akan langsung siap digunakan

Menggambar Objek

Pilih Alat: Klik salah satu tombol alat gambar (Titik, Garis, Persegi, Ellipse)
Atur Warna: Pilih warna menggunakan color picker
Atur Ketebalan: Masukkan nilai ketebalan garis (1-20)
Gambar:

Titik: Klik di canvas untuk membuat titik
Garis/Persegi/Ellipse: Drag dari titik awal ke titik akhir



Melakukan Transformasi

Pilih Objek: Klik pada objek di canvas atau di daftar objek
Pilih Jenis Transformasi:

Translasi: Masukkan nilai X dan Y, lalu klik "Pindah"
Rotasi: Masukkan sudut dalam derajat, lalu klik "Putar"
Scaling: Masukkan faktor skala X dan Y, lalu klik "Skala"


Transformasi Cepat: Gunakan tombol shortcut untuk transformasi umum

Mengelola Objek

Melihat Daftar: Scroll pada panel "Daftar Objek"
Memilih Objek: Klik pada objek di daftar atau di canvas
Menghapus: Klik "Hapus Terpilih" atau "Hapus Semua"

🛠️ Teknologi yang Digunakan

HTML5 Canvas: Untuk rendering grafik 2D
JavaScript ES6: Logika aplikasi dan manipulasi objek
CSS3: Styling dan layout responsif
Object-Oriented Programming: Struktur kode yang modular

📁 Struktur Kode
Class DrawingObject
javascriptclass DrawingObject {
    constructor(type, x, y, width, height, color, thickness)
    draw(context, isSelected)
    contains(x, y)
    translate(dx, dy)
    rotate(angle, centerX, centerY)
    scale(scaleX, scaleY, centerX, centerY)
}
Fungsi Utama

setTool(): Mengatur alat gambar aktif
startDrawing(), draw(), stopDrawing(): Handle event menggambar
selectObject(): Memilih objek
applyTranslation(), applyRotation(), applyScaling(): Transformasi
redrawCanvas(): Render ulang canvas

🎯 Fitur Transformasi Detail
1. Translasi (Translation)

Memindahkan objek ke koordinat baru
Input: nilai X dan Y untuk perpindahan
Rumus: x_baru = x_lama + dx, y_baru = y_lama + dy

2. Rotasi (Rotation)

Memutar objek terhadap titik pusatnya
Input: sudut dalam derajat
Menggunakan matriks rotasi 2D

3. Scaling

Mengubah ukuran objek
Input: faktor skala untuk X dan Y
Mempertahankan posisi relatif terhadap titik pusat

4. Transformasi Cepat

Kiri/Kanan/Atas/Bawah: Translasi 20 pixel
Putar 90°: Rotasi tetap 90 derajat
Besar/Kecil: Scaling 1.2x atau 0.8x

🎨 Antarmuka Pengguna
Layout Responsif

Header: Judul dan deskripsi aplikasi
Toolbar: Alat gambar dan pengaturan
Canvas: Area menggambar utama
Panel Transformasi: Kontrol transformasi objek
Daftar Objek: Manajemen objek

Visual Feedback

Status Bar: Informasi real-time tentang aktivitas
Object Highlighting: Objek terpilih ditampilkan dengan shadow
Preview Mode: Pratinjau objek saat menggambar
Responsive Design: Tampilan menyesuaikan ukuran layar

🔍 Deteksi Collision
Setiap objek memiliki metode contains(x, y) untuk mendeteksi apakah koordinat tertentu berada di dalam objek:

Titik: Menggunakan jarak euclidean
Garis: Menggunakan jarak titik ke garis
Persegi: Hit testing rectangular bounds
Ellipse: Menggunakan persamaan ellipse

💡 Tips Penggunaan

Menggambar Presisi: Gunakan koordinat yang ditampilkan di status bar
Transformasi Bertahap: Lakukan transformasi kecil-kecil untuk hasil yang presisi
Organisasi Objek: Gunakan daftar objek untuk navigasi yang mudah
Eksperimen: Coba kombinasi berbagai transformasi untuk efek menarik

🐛 Troubleshooting
Masalah Umum

Objek tidak terpilih: Pastikan mengklik tepat pada objek
Transformasi tidak bekerja: Pilih objek terlebih dahulu
Canvas kosong: Pastikan menggunakan drag untuk menggambar (kecuali titik)

Browser Compatibility

Chrome: ✅ Fully supported
Firefox: ✅ Fully supported
Safari: ✅ Fully supported
Edge: ✅ Fully supported

📝 Catatan Pengembangan
Aplikasi ini menggunakan HTML5 Canvas API dan JavaScript vanilla tanpa library eksternal, sehingga:

Performa optimal
Kompatibilitas browser yang baik
Mudah di-customize dan dikembangkan
Tidak memerlukan instalasi dependency

🚀 Pengembangan Lanjutan
Ide untuk fitur tambahan:

Export/Import objek ke format JSON
Undo/Redo functionality
Layer management
Gradient dan pattern fill
Bezier curves dan polygon tools
Snap to grid
Copy/paste objek

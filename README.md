# Refleksi Tutorial 11
## Hello Minikube
1. Yang saya lihat di log sebelum project diexpose sebagai Service adalah entri log dari aplikasi yang di-run di container. Sedangkan setelah diexpose sebagai Service, log yang muncul menggambarkan komunikasi antar service dan client. Jumlah log juga selalu bertambah ketika saya membuka aplikasi. Hal ini karena setiap saya membuka aplikasi, akan ada HTTP request baru yang masuk ke dalam entri log.

2. Tujuan dari adanya `-n` option adalah untuk menentukan namespace dalam menjalankan kubernetes. Hal ini digunakan untuk melakukan filter seperti partisi dan cluster. Jika tidak menggunakan opsi `-n`, resource yang dibuat pengguna akan ditampilkan secara eksplisit.

## Rolling Update & Kubernetes Manifest File
1. Perbedaan antara keduanya adalah recreate membutuhkan penghapusan dari pods lalu merecreate. Sedangkan rollback hanya perlu lakukan rollback.
2. Sudah dilakukan
3. Sudah dilakukan
4. Keuntungan menggunakan Kubernetes manifest files adalah adanya efisiensi karena hanya perlu menerapkan deployment manifest. 
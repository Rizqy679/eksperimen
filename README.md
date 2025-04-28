| Nama                    | NIM        | Kelas   | Matkul            |
|-------------------------|------------|---------|-------------------|
| Muhammad Rizqy | 312310415  | TI.23.A4| Pemrograman Web 2 |

1. Buat file HTML sederhana, misalnya eksperimen.html, dengan isi seperti ini:

![image](https://github.com/user-attachments/assets/c10ef0b3-ddad-42fa-9552-25eed6b1f1ca)

2. Buka file tersebut di browser.

![image](https://github.com/user-attachments/assets/0c7712dc-86db-4b6f-994c-1141b19a05c9)

3. isi form dengan teks biasa.

![image](https://github.com/user-attachments/assets/50f8c620-905a-46df-a780-0aac4de11109)

hasilnya akan muncul dengan aman.

![image](https://github.com/user-attachments/assets/1bad235e-6e5f-4716-a975-374417512590)

4. Uji dengan input skrip jahat.
   Masukkan ini ke kolom pencarian
   
   <script>alert('XSS Berhasil!')</script>

![image](https://github.com/user-attachments/assets/8ca33eec-4745-4bad-80f5-1920a0640b8f)
   
   Lalu klik cari.
   Browser akan menampilkan alert popup bertuliskan XSS Berhasil!.

![image](https://github.com/user-attachments/assets/7c66e6c1-af64-4518-98b0-45ae980de22f)

Cara Mencegahnya

Daripada menggunakan innerHTML.
   
![image](https://github.com/user-attachments/assets/22d81e6d-b08d-4113-8df3-ca22199456ac)

sebaiknya gunakan textContent.
   
![image](https://github.com/user-attachments/assets/69229158-41cd-40e0-a54c-cf683983b1a1)

Dengan textContent, input pengguna dianggap teks biasa, bukan HTML, sehingga aman dari XSS.

Hasil :

![image](https://github.com/user-attachments/assets/89f5355e-5c7c-4893-8908-030cd06c10e0)

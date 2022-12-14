[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-c66648af7eb3fe8bc4f294546bfd86ef473780cde1dea487d3c4ff354943c9ae.svg)](https://classroom.github.com/online_ide?assignment_repo_id=7737086&assignment_repo_type=AssignmentRepo)
# Graded Challenge 2

_Graded Challenge ini dibuat guna mengevaluasi pembelajaran pada Hacktiv8 Data Science Fulltime Program khususnya pada Linear Algebra dan Calculus._

---

## Dataset Description

* Pada graded challenge ini, anda diminta melakukan image processing menggunakan konsep linear algebra dan kalkulus.

* Dataset yang digunakan adalah sebuah gambar yang dapat diunduh [disini](https://cdn.cnn.com/cnnnext/dam/assets/201030094143-stock-rhodesian-ridgeback-exlarge-169.jpg).

*Sumber gambar: [link](https://edition.cnn.com/2020/10/30/world/dog-dna-intl-scli-gbr-scn/index.html)*

## Assignment Instructions

*Graded Challenge 2* dikerjakan dalam format ***notebook*** dengen beberapa **kriteria wajib** di bawah ini:

1. Gunakan library **Numpy** untuk kebutuhan pengolahan tipe data array dan beberapa operasi matematika.

2. Jika diperlukan, silahkan menggunakan library **Scipy**, **Numpy**, **Sympy** atau lainnya untuk melakukan perhitungan matematika.

3. Gunakan library **PIL** untuk membaca dan pengolahan gambar.

4. Untuk visualisasi, gunakan library **Matplotlib**.

5. *Objektif* dari project ini adalah **mendeteksi edge suatu gambar dan melakukan operasi perkalian matriks**. Sebagai petunjuk, berikut langkah-langkah untuk mengerjakan Graded Challenge 2 :
    
    1. Hitung vektor gradien (turunan parsial) masing-masing pixel untuk masing-masing sumbu x dan y dengan rumus <img src="http://www.sciweavers.org/tex2img.php?eq=%5Cfrac%7B%5Cpartial%20I%7D%7B%5Cpartial%20x%7D%20&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt="\frac{\partial I}{\partial x} " width="25" height="43" /> dan <img src="http://www.sciweavers.org/tex2img.php?eq=%5Cfrac%7B%5Cpartial%20I%7D%7B%5Cpartial%20y%7D%20&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt="\frac{\partial I}{\partial y} " width="24" height="46" />
    
    2. Hitung gradient magnitude tiap pixel dengan rumus <img src="http://www.sciweavers.org/upload/Tex2Img_1645323606/render.png"/>
    
    3. Tentukan sebuah threshold, misalkan `30`.

    4. Jika nilai magnitude melebihi angka threshold, maka edge terdeteksi.
    
    5. Buat minimal dua buah threshold lain sehingga jumlah minimal threshold adalah 3. Lakukan poin 4. Visualisasikan hasil edge dari masing-masing threshold.

    6. Tentukan nilai threshold terbaik berdasarkan percobaan poin 5 diatas. Narasikan analisa yang dibuat.

    7. Buat sebuah matriks dengan nilai apapun yang bersesuaian dengan ukuran gambar dan sesuai dengan aturan perkalian matriks.

    8. Matriks ini kemudian akan dilakukan perkalian dengan matriks edge dengan threshold terbaik. Visualisasikan dan narasikan hasil dari perkalian kedua matriks ini.

6. **Catatan**: Anda dapat menggunakan metode apapun, baik menggunakan library atau melakukan perhitungan dengan metode numerik.

7. *Project* dinyatakan selesai dan diterima untuk dinilai jika saat dilakukan `Run All` pada *notebook*, semua *cell* berhasil tereksekusi sampai akhir.

8. Isi *notebook* harus mengikuti *outline* di bawah ini:
   
   1. Perkenalan
      > Bab pengenalan harus diisi dengan identitas, *metode* yang ingin dilakukan guna mencapai tujuan.
   
   2. Import pustaka yang dibutuhkan
      > *Cell* pertama pada *notebook* **harus berisi dan hanya berisi** semua *library* yang digunakan dalam *project*.
   
   3. Data Loading
      > Bagian ini berisi proses *data loading* yang kemudian dilanjutkan dengan *explorasi data* secara sederhana.
   
   4. Data Cleaning
      > Bagian ini berisi proses penyiapan data berupa data cleaning sebelum dilakukan pemrosesan lebih lanjut. Proses cleaning dapat berupa memberi filtering komponen warna, mengubah gambar warna menjadi grayscale, dan lain sebagainya.
   
   5. Image Processing
      > Bagian ini berisi kode-kode serta perhitungan-perhitungan untuk mencapai tujuan.
   
   6. Hasil dan Kesimpulan
      > Pada bab terakhir ini, **harus berisi** kesimpulan yang mencerminkan hasil yang didapat dengan membandingkan beberapa nilai threshold dan juga hasil perkalian matriks yang telah dilakukan (dalam visualisasi gambar).

10. *Notebook* harus diupload dalam akun GitHub masing-masing siswa untuk selanjutnya dinilai.

## Assignment Submission

- Simpan assignment pada sesi ini dengan nama `h8dsft_P0W2_<nama-student>.ipynb`, misal `h8dsft_P0W2_raka_ardhi.ipynb`.
- Push Assigment yang telah kalian buat ke akun Github masing-masing student.

## Assignment Objectives

*Graded Challenge 2* ini dibuat guna mengevaluasi Linear Algebra dan Calculus sebagai berikut:

- Mampu memuat data gambar
- Mampu melakukan transformasi tipe data gambar ke data yang siap olah
- Mampu melakukan eksplorasi data gambar
- Mampu menerapkan konsep kalkulus pada pengolahan citra menggunakan library atau metode numerik from scratch
- Mampu menerapkan konsep linear algebra pada pengolahan citra menggunakan library atau metode numerik from scratch
- Mampu memvisualisasikan gambar menggunakan matplotlib

---

## Assignment Rubrics

### Code Review

| Criteria | Meet Expectations | Points |
| --- | --- | --- |
| Data Loading | Mampu memuat data gambar dengan library PIL | 2 pts |
| Data Transformation | Mampu mentransformasikan gambar ke array | 2 pts |
| Image Data Exploration | Mampu mengeksplorasi data gambar dan mengambil keputusan dalam menindaklanjut data | 3 pts |
| Calculus Implementation | Mampu menerapkan perhitungan turunan parsial/vector gradient dalam kode | 10 pts |
| Linear Algebra Implementation | Mampu menerapkan operasi perkalian matriks dalam kode | 10 pts |
| Image Visualization | Mampu memvisualisasikan gambar dengan Matplotlib | 3 pts |

### Readability

| Criteria | Meet Expectations | Points |
| --- | --- | --- |
| Tertata Dengan Baik | Semua baris kode terdokumentasi dengan baik dengan menggunakan Markdown untuk penjelasan kode. | 10 pts |

### Analysis

| Criteria | Meet Expectations | Points |
| --- | --- | --- |
| Overall Analysis | Menarik informasi/kesimpulan dari perbandingan nilai threshold (minimal 3 nilai threshold berbeda) | 10 pts |

---

```
Total Points : 50
```

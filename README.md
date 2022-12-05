[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-c66648af7eb3fe8bc4f294546bfd86ef473780cde1dea487d3c4ff354943c9ae.svg)](https://classroom.github.com/online_ide?assignment_repo_id=8296170&assignment_repo_type=AssignmentRepo)
# Live Code 3

## Instruction

Live Code ini dikerjakan dalam format ***notebook*** dan push file notebook pekerjaannya ke <strong>repository soal</strong>. **Beri nama file dengan: h8_p0lc3_NAMA.ipynb**

---

## Problem

Kamu adalah seorang data scientist di salah satu perusahaan asuransi. Saat ini, kamu sedang membuat model machine learning untuk memprediksi apakah klaim asuransi perjalanan seseorang diterima atau tidak berdasarkan beberapa parameter.

Sebelum melakukan modelling, tahapan yang harus dilakukan adalah *eksploratory data analysis*, dimana kamu akan mengksplorasi data untuk mengenal lebih dalam pola dari data sebelum melakukan tahapan selanjutnya.

Dataset yang akan digunakan tersimpan dalam database MySQL yang akan kamu akses melalui Python menggunakan library `mysql.connector`. Berikut deskripsi kolom-kolom pada tabel:

**Nama Tabel: travel_insurance**
- Name of agency (agency)
- Type of travel insurance agencies (agency_type)
- Distribution channel of travel insurance agencies (distribution_channel)
- Name of the travel insurance products (product_name)
- Claim Status, Yes/No (claim)
- Duration of travel (duration)
- Destination of travel (destination)
- Amount of sales of travel insurance policies (net_sales)
- Commission received for travel insurance agency (commission)
- Gender of insured (gender)
- Age of insured (age)

Untuk mengakses tabel tersebut, gunakan informasi di bawah berikut:

```
  host      = remotemysql.com
  user      = cESOsiaUiy
  passwd    = saecUeCNAL
  database  = cESOsiaUiy
```

**Pastikan ada koneksi internet, karena server MySQL tersebut online dan pastikan bahwa tiap cell ada pendefinisian koneksi server MySQL dan pendefinisian kursor. Kamu bisa gunakan `pd.read_sql_query(query,connection)` untuk langsung menampilkan query dalam dataframe.** (Selengkapnya dapat lihat pada link [berikut](https://stackoverflow.com/questions/64565904/how-to-use-pd-read-sql-using-mysql-connector) sebagai referensi.

Supaya mudah dalam melakukan exploratory data analysis, kita perlu membuat penjabaran masalah dan kemudian dapat disimpulkan. Namun, sebelum membuat penjabaran masalah, pastikan sudah menentukan *problem statement* agar kesimpulan yang dibuat lebih terarah.

### **PROBLEM STATEMENT**
1. Definisikan problem statement berdasarkan penjabaran masalah di bawah yang akan teman-teman jawab menggunakan SQL!

### **Penjabaran Masalah **
1. Tampilkan tabel sampai 5 baris pertama
2. Berasal dari agensi travel mana saja nasabah yang klaim asuransi?
3. Tipe agensi apa yang paling banyak yang klaim asuransinya diterima?
4. Destinasi negara mana yang paling banyak diterima klaim asuransinya?
5. Berapa nilai minimum, maksimum, dan rata-rata usia yang pengajuan klaim asuransinya diterima?
6. Jika agen asuransi hanya mengurusi klaim yang tujuan negaranya Singapura, Thailand, dan Malaysia, berapa total komisi yang didapat dari klaim yang diterima? (anggap komisi dalam USD)

**PERHATIKAN:** untuk nomor 2-6, tiap nomor diharuskan ada insight yang disampaikan. Tidak perlu membuat plot/data visualisasi. Hanya tampilkan berupa dataframe (langsung hasil dari query)!

### **Poin Analisis**
1. Dari penjabaran yang sudah kamu bahas (pertanyaan 2-6), apa kesimpulan yang kamu dapat sampaikan?

---

## Assignment Rubrics

### 1. Code Review
**Impementasi Code Python**
|No.|Criteria|Meet Expectations|Points|
|--- |--- |--- |--- |
|a|Data Connection|Mampu menghubungkan database pada server MySQL ke Python| 5 pts |
|b|SQL Queries|Mampu mengolah data sampai siap dianalisa meliputi data cleaning dan missing value checking/handling | 5 pts each (30 pts max) |

### 2. Conceptual & Analysis
**Menjawab Pertanyaan**
|No.|Criteria|Meet Expectations|Points|
|--- |--- |--- |--- |
|a|Problem Statement|Mampu mendefinisikan problem statement| 5 pts |
|b|Insights|Mampu memberikan kesimpulan/insight dari masing-masing penjabaran (poin penjabaran 2-6) | 7 pts each (35 pts max) |
|c|Overall Analysis|Mampu memberikan kesimpulan/insight dari penjabaran dan problem statement pada poin analisis| 15 pts |

### 3. Readability

|Criteria|Meet Expectations|Points|
|--- |--- |--- |
|Tertata Dengan Baik|Semua Cell Di Notebook Terdokumentasi Dengan Baik Dengan Markdown Pada Tiap Cell Untuk Penjelasan Kode dan **Format Notebook Sesuai dengan Template**.| 10 pts |

---

```{admonition} Total Points
**100**
```

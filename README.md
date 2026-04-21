<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:00d9ff,100:7c3aed&height=200&section=header&text=Dzakwan%20Avue%20Rahmani&fontSize=40&fontColor=ffffff&fontAlignY=38&desc=Sistem%20Informasi%20%7C%20NIM%20515241005&descSize=16&descAlignY=58&descColor=a0aec0" />

</div>

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=00D9FF&center=true&vCenter=true&width=500&lines=Database+Developer;SQL+Enthusiast;Sistem+Informasi+Student;Data+is+Everything+%F0%9F%97%84%EF%B8%8F)](https://git.io/typing-svg)

</div>

---

## 👋 Tentang Saya

```sql
SELECT * FROM mahasiswa WHERE nama = 'Dzakwan Avue Rahmani';
```

```
+------------------+-----------------------------+
| Field            | Value                       |
+------------------+-----------------------------+
| Nama             | Dzakwan Avue Rahmani        |
| NIM              | 515241005                   |
| Program Studi    | Sistem Informasi            |
| Keahlian Utama   | Database & SQL              |
| Status           | Aktif ✅                    |
+------------------+-----------------------------+
```

---

## 🛠️ Tech Stack

<div align="center">

![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

</div>

---

## 🗄️ Keahlian Database

| Skill | Level |
|-------|-------|
| SQL Query & DML | ████████░░ 88% |
| Database Design & ERD | ████████░░ 82% |
| Query Optimization | ███████░░░ 75% |
| Data Analysis (CTE, Window Func) | ███████░░░ 79% |
| Stored Procedure & Trigger | ███████░░░ 76% |
| Python + SQLAlchemy | ██████░░░░ 65% |

---

## 💼 Proyek Unggulan

### 🏪 Sistem Manajemen Inventori Toko
> Database lengkap untuk sistem retail — produk, stok, supplier, laporan penjualan harian.
`MySQL` `Stored Procedure` `Trigger` `ERD`

### 🎓 Database Akademik Mahasiswa
> Skema relasional ternormalisasi (BCNF) — KRS, nilai, jadwal, transkrip akademik.
`PostgreSQL` `Normalisasi` `View` `Window Functions`

### 📈 Analisis Data Penjualan E-Commerce
> Query analitik dengan CTE & window functions untuk insight bisnis dari data transaksi.
`SQL Server` `CTE` `Data Analysis` `Reporting`

---

## ✍️ SQL Snippet Favorit

```sql
-- Top 3 produk per kategori bulan ini
WITH ranked AS (
  SELECT
    p.nama_produk,
    k.nama_kategori,
    SUM(d.qty * d.harga) AS total,
    RANK() OVER (PARTITION BY k.kategori_id ORDER BY SUM(d.qty * d.harga) DESC) AS rnk
  FROM detail_penjualan d
  JOIN produk p ON d.produk_id = p.produk_id
  JOIN kategori k ON p.kategori_id = k.kategori_id
  WHERE d.tanggal >= DATE_TRUNC('month', CURRENT_DATE)
  GROUP BY p.produk_id, k.kategori_id
)
SELECT nama_kategori, nama_produk, total
FROM ranked WHERE rnk <= 3;
```

---

## 📊 GitHub Stats

<div align="center">

![dzakwanavie's GitHub Stats](https://github-readme-stats.vercel.app/api?username=dzakwanavie&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=00d9ff&icon_color=7c3aed&text_color=e8eaf0)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=dzakwanavie&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=00d9ff&text_color=e8eaf0)

</div>

---

## 📫 Hubungi Saya

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-dzakwanavie-181717?style=for-the-badge&logo=github)](https://github.com/dzakwanavie)
[![Email](https://img.shields.io/badge/Email-Kirim%20Pesan-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:dzakwan@email.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/dzakwanavie)

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7c3aed,50:00d9ff,100:0d1117&height=120&section=footer" />

<sub>⚡ "Good data structure is the foundation of great software." — Dzakwan Avue Rahmani</sub>

</div>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,40:1a1a2e,80:16213e,100:0f3460&height=220&section=header&text=Dzakwan%20Avie%20Rahmani&fontSize=42&fontColor=e2e8f0&fontAlignY=38&desc=Sistem%20Informasi%20%E2%80%A2%20NIM%20515241005&descSize=17&descAlignY=58&descColor=94a3b8&animation=fadeIn" />

</div>

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=20&pause=1000&color=38BDF8&center=true&vCenter=true&width=540&lines=SELECT+*+FROM+skills+WHERE+level+%3D+'Expert';Database+Designer+%26+SQL+Developer;Sistem+Informasi+%E2%80%94+Angkatan+2024;Data+Structures+%7C+ERD+%7C+Query+Optimization)](https://git.io/typing-svg)

</div>

<br>

---

## 🧬 Profil Mahasiswa

```sql
/* ================================================
   QUERY: Identitas Mahasiswa
   DATABASE: Universitas — Sistem Informasi
   ================================================ */

SELECT
    nim,
    nama_lengkap,
    program_studi,
    keahlian_utama,
    status_akademik
FROM
    mahasiswa
WHERE
    nim = '515241005';
```

<div align="center">

| 🏷️ Field | 📋 Value |
|:---|:---|
| **NIM** | `515241005` |
| **Nama** | Dzakwan Avie Rahmani |
| **Program Studi** | Sistem Informasi |
| **Keahlian Utama** | Database & SQL Development |
| **Status** | Aktif ✅ |

</div>

---

## 🛠️ Tech Stack

<div align="center">

![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)

</div>

---

## 🗄️ Database Skills

```
SQL Query & DML            ████████░░  88%
Database Design & ERD      ████████░░  82%
Data Analysis (CTE/Window) ███████░░░  79%
Query Optimization         ███████░░░  75%
Stored Procedure & Trigger ███████░░░  76%
Normalisasi (1NF–BCNF)     ████████░░  80%
PHP + MySQL Integration    ██████░░░░  65%
```

---

## 💼 Proyek Unggulan

### 🏫 Sistem Absensi Madrasah
> Aplikasi absensi berbasis web untuk madrasah — mencakup data kehadiran siswa/pegawai, honorarium, dan laporan penggajian pegawai secara otomatis.

**Stack:** `MySQL` `PHP` `Stored Procedure` `Trigger` `ERD`

🔗 **Live Demo:** [mtsnk.infinityfree.me](http://mtsnk.infinityfree.me)

---

### 🎓 Database Akademik Mahasiswa
> Skema relasional ternormalisasi (BCNF) — KRS, nilai, jadwal, dan transkrip akademik.

**Stack:** `PostgreSQL` `Normalisasi` `View` `Window Functions`

---

## ✍️ SQL Snippet Favorit

```sql
-- ============================================
-- Top 3 pegawai dengan kehadiran terbaik bulan ini
-- ============================================
WITH ranked_pegawai AS (
    SELECT
        p.nama_pegawai,
        d.nama_divisi,
        COUNT(a.id_absensi)                           AS total_hadir,
        RANK() OVER (
            PARTITION BY d.id_divisi
            ORDER BY COUNT(a.id_absensi) DESC
        )                                             AS peringkat
    FROM   absensi      a
    JOIN   pegawai      p ON a.id_pegawai = p.id_pegawai
    JOIN   divisi       d ON p.id_divisi  = d.id_divisi
    WHERE  a.tanggal >= DATE_TRUNC('month', CURRENT_DATE)
      AND  a.status   = 'Hadir'
    GROUP  BY p.id_pegawai, p.nama_pegawai, d.id_divisi, d.nama_divisi
)
SELECT
    nama_divisi,
    nama_pegawai,
    total_hadir
FROM   ranked_pegawai
WHERE  peringkat <= 3
ORDER  BY nama_divisi, peringkat;
```

---

## 📊 GitHub Stats

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=dzakwanavie&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=38bdf8&icon_color=818cf8&text_color=e2e8f0&count_private=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=dzakwanavie&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=38bdf8&text_color=e2e8f0)

![GitHub Streak](https://streak-stats.demolab.com?user=dzakwanavie&theme=tokyonight&hide_border=true&background=0d1117&ring=38bdf8&fire=818cf8&currStreakLabel=38bdf8)

</div>

---

## 📫 Hubungi Saya

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-dzakwanavie-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/dzakwanavie)
[![Instagram](https://img.shields.io/badge/Instagram-@thrskye-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/thrskye?igsh=MWE2ODY2anBuajgzMg==)
[![Email](https://img.shields.io/badge/Email-dzakwanavie@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:dzakwanavie@gmail.com)

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f3460,40:16213e,80:1a1a2e,100:0d1117&height=130&section=footer" />

<sub>⚡ <i>"Good data structure is the foundation of great software."</i></sub><br>
<sub>— Dzakwan Avie Rahmani · Sistem Informasi · 515241005</sub>

</div>

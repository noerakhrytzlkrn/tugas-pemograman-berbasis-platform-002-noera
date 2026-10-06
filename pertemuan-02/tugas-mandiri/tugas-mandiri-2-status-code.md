# Tugas Mandiri 2 - Memahami HTTP Status Code

## Hasil Pengujian

| Status Code | Arti | Hasil Pengujian | Kapan Digunakan |
|---|---|---|---|
| 200 | OK | Server mengembalikan 200 OK | Digunakan ketika request berhasil diproses oleh server. |
| 201 | Created | Server mengembalikan 201 Created | Digunakan ketika request berhasil dan menghasilkan resource baru. |
| 400 | Bad Request | Server mengembalikan 400 Bad Request | Digunakan ketika request dari client tidak valid atau salah format. |
| 401 | Unauthorized | Server mengembalikan 401 Unauthorized | Digunakan ketika client belum melakukan autentikasi atau kredensial tidak valid. |
| 403 | Forbidden | Server mengembalikan 403 Forbidden | Digunakan ketika client tidak memiliki izin untuk mengakses resource. |
| 404 | Not Found | Server mengembalikan 404 Not Found | Digunakan ketika resource atau endpoint yang diminta tidak ditemukan. |
| 500 | Internal Server Error | Server mengembalikan 500 Internal Server Error | Digunakan ketika terjadi kesalahan internal pada sisi server. |

## Pertanyaan

### 1. Apa perbedaan 400 dan 404?
Status 400 Bad Request terjadi ketika request yang dikirim oleh client tidak valid atau memiliki format yang salah. Sementara itu, status 404 Not Found terjadi ketika resource atau endpoint yang diminta tidak ditemukan pada server.

### 2. Apa perbedaan 401 dan 403?
Status 401 Unauthorized terjadi ketika client belum melakukan autentikasi atau kredensial yang diberikan tidak valid. Sedangkan status 403 Forbidden terjadi ketika server memahami request, tetapi client tidak memiliki izin untuk mengakses resource tersebut.

### 3. Mengapa 500 menunjukkan masalah pada sisi server?
Status 500 Internal Server Error menunjukkan bahwa server mengalami kesalahan internal saat memproses request sehingga request tidak dapat diselesaikan dengan semestinya.

### 4. Apakah semua error HTTP berarti server mengalami kerusakan?
Tidak. Tidak semua error HTTP berarti server mengalami kerusakan. Status 4xx umumnya menunjukkan masalah pada request dari client, sedangkan status 5xx menunjukkan adanya masalah pada sisi server.

## Screenshot Hasil Pengujian

![Status 200](../../kegiatan-praktikum/screenshots/status-200-httpbin.jpg)

![Status 404](../../kegiatan-praktikum/screenshots/status-404-httpbin.jpg)

![Status 500](../../kegiatan-praktikum/screenshots/status-500-httpbin.jpg)
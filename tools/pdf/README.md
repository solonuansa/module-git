# Build PDF Markdown

Folder ini berisi seluruh alat konversi Markdown ke PDF untuk repository modul Git.

## Isi Folder

- `export-pdf.ps1`
  Skrip utama build PDF.
- `md-to-pdf.config.js`
  Konfigurasi `md-to-pdf`.
- `pdf-style.css`
  Styling PDF.
- `prepare_markdown_for_pdf.py`
  Menyiapkan markdown sementara untuk proses render.
- `update_toc_pages.py`
  Menyinkronkan nomor halaman daftar isi.
- `fix_pdf_links.py`
  Memperbaiki link internal PDF dan menambahkan bookmark.

## Build dari Root Repository

Jalankan dari root repository:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\pdf\export-pdf.ps1
```

Untuk file tertentu:

```powershell
powershell -ExecutionPolicy Bypass -File .\tools\pdf\export-pdf.ps1 -InputFile "tutorial-instalasi-git.md"
```

## Build dari Folder `tools/pdf`

Kalau sedang berada di folder ini:

```powershell
powershell -ExecutionPolicy Bypass -File .\export-pdf.ps1 -InputFile "draft_Module_Git.md"
```

Input file tetap dibaca relatif terhadap root repository, jadi nama file Markdown cukup ditulis seperti biasa.

## Yang Dilakukan Script

1. Membuat versi markdown sementara untuk keperluan PDF.
2. Merender PDF dengan `md-to-pdf`.
3. Membaca nomor halaman hasil render.
4. Memperbarui blok `Daftar Isi` pada markdown sumber.
5. Mengulang render sampai nomor halaman daftar isi stabil.
6. Memperbaiki link internal PDF.
7. Menambahkan bookmark PDF berdasarkan heading utama.

## Kebutuhan

- PowerShell
- Node.js dan `npx`
- Python 3
- Paket Python `pypdf`

## Catatan

- File Markdown utama tetap diletakkan di root repository.
- Hasil PDF selalu dibuat berdampingan dengan file Markdown sumber.
- Marker `<!-- AUTO-TOC:START -->` dan `<!-- AUTO-TOC:END -->` jangan dihapus jika ingin sinkronisasi daftar isi tetap otomatis.

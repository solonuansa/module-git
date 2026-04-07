# Tutorial Instalasi Git pada Windows dan macOS

Dokumen ini merangkum panduan instalasi Git untuk Windows dan macOS dalam satu file. Ikuti bagian yang sesuai dengan sistem operasi yang Anda gunakan, lalu lanjutkan ke bagian verifikasi dan konfigurasi awal.

## Daftar Isi

<!-- AUTO-TOC:START -->
[Persiapan](#1-persiapan) (hal. 1)  
[Instalasi Git di Windows](#2-instalasi-git-di-windows) (hal. 1)  
[Instalasi Git di macOS](#3-instalasi-git-di-macos) (hal. 10)  
[Verifikasi Instalasi](#4-verifikasi-instalasi) (hal. 11)  
[Konfigurasi Awal Git](#5-konfigurasi-awal-git) (hal. 12)  
<!-- AUTO-TOC:END -->

---

## 1. Persiapan

Sebelum mulai, siapkan hal-hal berikut:

- Koneksi internet untuk mengunduh installer atau paket instalasi.
- Hak akses instalasi pada komputer yang digunakan.
- Aplikasi terminal:
  - Windows: Command Prompt, PowerShell, atau Git Bash.
  - macOS: Terminal.
- Editor teks untuk bekerja dengan file Git. Untuk Windows, editor yang disarankan adalah [Visual Studio Code](https://code.visualstudio.com/), [Notepad++](https://notepad-plus-plus.org/), atau [Vim](https://www.vim.org/).

Tautan unduhan resmi:

- Windows: <https://git-scm.com/download/win>
- macOS: <https://git-scm.com/download/mac>

## 2. Instalasi Git di Windows

Berikut langkah-langkah instalasi Git menggunakan installer resmi pada Windows.

<ol class="step-list">
  <li>
    <div class="step-card">
      <p>Unduh Git dari situs resmi, lalu klik dua kali file installer yang sudah diunduh. Saat jendela lisensi muncul, klik <strong>Next</strong>.</p>
      <figure class="step-figure">
        <img src="images/01/install-01.jpg" alt="Langkah 1">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Tentukan lokasi instalasi. Secara default, Git akan dipasang di <code>C:\Program Files\Git</code>. Jika tidak ada kebutuhan khusus, gunakan lokasi default lalu klik <strong>Next</strong>.</p>
      <figure class="step-figure">
        <img src="images/01/install-02.jpg" alt="Langkah 2">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Pada pilihan komponen, gunakan pengaturan default, lalu klik <strong>Next</strong>.</p>
      <figure class="step-figure">
        <img src="images/01/install-03.jpg" alt="Langkah 3">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Tentukan nama folder shortcut di Start Menu. Gunakan nilai default (<code>Git</code>) atau sesuaikan bila diperlukan, kemudian lanjutkan.</p>
      <figure class="step-figure">
        <img src="images/01/install-04.jpg" alt="Langkah 4">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Pilih editor teks yang akan digunakan bersama Git. Anda bebas memilih editor yang tersedia.</p>
      <figure class="step-figure">
        <img src="images/01/install-05-01.jpg" alt="Langkah 5a">
      </figure>
      <p>Beberapa editor yang umum digunakan ditampilkan pada daftar berikut.</p>
      <figure class="step-figure">
        <img src="images/01/install-05-02.jpg" alt="Langkah 5b">
      </figure>
      <p>Jika editor yang Anda gunakan tidak ada dalam daftar, pilih opsi terakhir lalu arahkan ke file executable editor tersebut.</p>
      <figure class="step-figure">
        <img src="images/01/install-05-03.jpg" alt="Langkah 5c">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Pada pengaturan nama branch default untuk repository baru, pilih <strong>Override the default branch name for new repositories</strong> lalu gunakan <code>main</code>.</p>
      <figure class="step-figure">
        <img src="images/01/install-06.jpg" alt="Langkah 6">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Pada pengaturan PATH environment, pilih opsi yang memungkinkan Git digunakan dari <strong>Git Bash</strong> dan juga <strong>Command Prompt</strong>.</p>
      <figure class="step-figure">
        <img src="images/01/install-07.jpg" alt="Langkah 7">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Untuk HTTPS transport backend, pilih <strong>Use the native Windows Secure Channel library</strong>.</p>
      <figure class="step-figure">
        <img src="images/01/install-08.jpg" alt="Langkah 8">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Pada pengaturan line ending conversions, gunakan opsi pertama agar kompatibilitas file teks tetap baik.</p>
      <figure class="step-figure">
        <img src="images/01/install-09.jpg" alt="Langkah 9">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Pada pemilihan terminal emulator untuk Git Bash, pilih <strong>Use MinTTY</strong>.</p>
      <figure class="step-figure">
        <img src="images/01/install-10.jpg" alt="Langkah 10">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Untuk perilaku standar <code>git pull</code>, gunakan opsi default <strong>Fast-forward or merge</strong>.</p>
      <figure class="step-figure">
        <img src="images/01/install-11.jpg" alt="Langkah 11">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Pada pengaturan credential helper, gunakan opsi default yang disarankan installer.</p>
      <figure class="step-figure">
        <img src="images/01/install-12.jpg" alt="Langkah 12">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Pada pilihan tambahan, aktifkan <strong>Enable file system caching</strong> lalu lanjutkan proses instalasi.</p>
      <figure class="step-figure">
        <img src="images/01/install-13.jpg" alt="Langkah 13">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Tunggu sampai proses instalasi selesai.</p>
      <figure class="step-figure">
        <img src="images/01/install-14.jpg" alt="Langkah 14">
      </figure>
    </div>
  </li>
  <li>
    <div class="step-card">
      <p>Jika instalasi selesai, klik <strong>Finish</strong>.</p>
      <figure class="step-figure">
        <img src="images/01/install-15.jpg" alt="Langkah 15">
      </figure>
    </div>
  </li>
</ol>

## 3. Instalasi Git di macOS

Pada macOS, Git dapat dipasang dengan beberapa cara. Pilih salah satu metode berikut sesuai kebutuhan Anda.

### 3.1 Metode 1: Xcode Command Line Tools

Metode ini cocok jika Anda ingin menggunakan paket pengembang bawaan Apple.

1. Buka aplikasi **Terminal**.
2. Jalankan perintah berikut:

    ```bash
    git --version
    ```

3. Jika Git belum tersedia, macOS biasanya akan menampilkan pop-up untuk menginstal **Command Line Developer Tools**.
4. Klik **Install** lalu setujui syarat instalasinya.
5. Tunggu sampai proses unduh dan instalasi selesai.

### 3.2 Metode 2: Homebrew

Metode ini cocok jika Anda ingin memasang Git versi terbaru melalui package manager.

1. Jika Homebrew belum terpasang, jalankan perintah berikut di Terminal:

    ```bash
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```

2. Setelah Homebrew terpasang, instal Git dengan perintah berikut:

    ```bash
    brew install git
    ```

3. Tunggu hingga Homebrew selesai mengunduh dan memasang Git.

### 3.3 Metode 3: Installer Binary

Metode ini menggunakan installer grafis, mirip seperti proses instalasi pada Windows.

1. Buka situs resmi Git untuk macOS di <https://git-scm.com/download/mac>.
2. Pilih installer yang tersedia. Biasanya Anda akan diarahkan ke penyedia file seperti SourceForge.
3. Unduh file installer berformat `.dmg`.
4. Buka file tersebut, lalu ikuti petunjuk instalasi yang tampil di layar sampai selesai.

## 4. Verifikasi Instalasi

Setelah instalasi selesai, pastikan Git sudah dapat digunakan dari terminal.

Jalankan perintah berikut:

```bash
git --version
```

Jika instalasi berhasil, terminal akan menampilkan informasi versi Git, misalnya:

```bash
git version 2.x.x
```

Pada Windows, Anda bisa menjalankan perintah ini melalui **Command Prompt**, **PowerShell**, atau **Git Bash**. Pada macOS, jalankan melalui **Terminal**.

## 5. Konfigurasi Awal Git

Setelah Git terpasang, lakukan konfigurasi identitas agar setiap commit memiliki nama dan email yang jelas.

1. Atur nama pengguna:

    ```bash
    git config --global user.name "Nama Lengkap Anda"
    ```

2. Atur alamat email:

    ```bash
    git config --global user.email "emailanda@example.com"
    ```

3. Periksa hasil konfigurasi:

    ```bash
    git config --list
    ```

Jika nama dan email sudah tampil pada hasil konfigurasi, Git siap digunakan.

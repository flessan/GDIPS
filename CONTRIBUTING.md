
<div align="center">

![Contributing](https://img.shields.io/badge/Welcome-Contributor-brightgreen?style=for-the-badge)
![Open Source](https://img.shields.io/badge/Type-Open_Source-informational?style=for-the-badge)

**Terima kasih sudah mau berkontribusi ke GDIPS!** 🎉

*Kapanpun kamu bisa mulai — tidak perlu jadi expert, yang penting mau belajar.*

[🇬🇧 English](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#english) · [🇮🇩 Bahasa Indonesia](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#bahasa-indonesia)

---

</div>

## Bahasa Indonesia

### 📋 Daftar Isi

- [Aturan Dasar](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-aturan-dasar)
- [Cara Berkontribusi](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-cara-berkontribusi)
- [Setup Development](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-setup-development)
- [Struktur Folder](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-struktur-folder)
- [Standar Kode](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-standar-kode)
- [Cara Membuat Pull Request](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-cara-membuat-pull-request)
- [Cara Melaporkan Bug](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-cara-melaporkan-bug)
- [Cara Mengusulkan Fitur](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-cara-mengusulkan-fitur)

---

### 📜 Aturan Dasar

> **Baca ini dulu sebelum apapun.**

1. **Hormati semua orang** — tidak ada toleransi untuk toxic, rasisme, atau bullying
2. **Komunikasi yang baik** — jelaskan masalah dengan jelas, sabar menunggu review
3. **Jangan copy-paste tanpa paham** — kita di sini untuk belajar
4. **Boleh salah** — bug itu wajar, yang penting mau diperbaiki
5. **Tanya jika bingung** — lebih baik bertanya daripada asal push

---

### 🛠 Cara Berkontribusi

```
Pilih jalur kontribusimu:

┌─────────────────────────────────────────────────┐
│                                                 │
│   💻  Kode           →  Fix bug / fitur baru    │
│   🐛  Bug Report     →  Laporkan masalah        │
│   💡  Ide            →  Usulkan fitur           │
│   📝  Dokumentasi    →  Tulis/edit docs         │
│   🎨  Design         →  UI/UX, assets           │
│   🌐  Terjemahan     →  Terjemahkan docs/UI     │
│   ⭐  Dukungan       →  Star & share repo       │
│                                                 │
└─────────────────────────────────────────────────┘
```

#### 💻 Kontribusi Kode

1. **Cari issue dengan label `good first issue`** atau `help wanted`
2. **Comment di issue**: "Saya mau kerjakan ini" (biar tidak dobel)
3. **Fork repo ini**
4. **Buat branch baru** dengan nama yang jelas:
   ```bash
   git checkout -b fix/login-crash
   git checkout -b feat/song-upload
   git checkout -b docs/contributing-guide
   ```
5. **Kerjakan perubahannya**
6. **Commit dengan pesan yang jelas** (lihat [Standar Commit](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/-#standar-commit))
7. **Push ke fork kamu**
8. **Buat Pull Request**

#### 🐛 Melaporkan Bug

Lihat [Cara Melaporkan Bug](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-cara-melaporkan-bug) di bawah.

#### 💡 Mengusulkan Fitur

Lihat [Cara Mengusulkan Fitur](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-cara-mengusulkan-fitur) di bawah.

#### 📝 Dokumentasi

- Salin kesalahan typo, kalimat membingungkan, atau info yang kurang
- Bisa langsung PR atau buat issue dengan label `documentation`
- Bahasa bebas (Indonesia/English), yang penting jelas

#### 🎨 Design & Assets

- Buka issue dengan label `design`
- Sertakan preview/gambar usulan kamu
- Format: PNG/SVG untuk icon, Figma link untuk layout

#### 🌐 Terjemahan

- Cek file yang belum diterjemahkan
- Buat PR dengan format nama file: `filename.id.md` (Indonesia)
- Jangan translate secara harfiah — sesuaikan konteks

---

### 🖥 Setup Development

#### Prasyarat

```
✅ PHP 7.4+ (8.0+ direkomendasikan)
✅ Web Server (Apache/XAMPP/Nginx)
✅ MySQL / MariaDB
✅ Git
✅ Text Editor (VS Code direkomendasikan)
✅ Akun Discord (untuk komunikasi)
```

#### Langkah Setup

```bash
# 1. Fork & Clone repo
git clone https://github.com/KAMU/GDIPS.git
cd GDIPS

# 2. Buat branch baru
git checkout -b fitur-kamu

# 3. Setup database
# Import gdips.sql ke MySQL kamu
# Edit config koneksi database di file config

# 4. Jalankan di local server
# Arahkan web server ke folder project

# 5. Mulai koding!
```

#### File Config Utama

```php
// Sesuaikan dengan environment kamu
define('DB_HOST', 'localhost');
define('DB_NAME', 'gdips_db');
define('DB_USER', 'root');
define('DB_PASS', '');
```

> ⚠️ **Jangan pernah push password atau kredensial asli!**

---

### 📁 Struktur Folder

```
GDIPS/
├── 📂 database/          # SQL schema & migrations
│   ├── gdips.sql
│   └── updates/
├── 📂 dashboard/         # Web dashboard
│   ├── index.php
│   ├── css/
│   └── js/
├── 📂 tools/             # Utility & experimental tools
├── 📂 songs/             # Uploaded songs storage
├── 📂 assets/            # Images, icons, resources
├── 📂 config/            # Configuration files
├── 📂 docs/              # Documentation
├── 📄 .github/           # GitHub templates & workflows
│   ├── ISSUE_TEMPLATE/
│   └── PULL_REQUEST_TEMPLATE.md
├── 📄 CONTRIBUTING.md    # File ini
├── 📄 LICENSE
└── 📄 README.md
```

---

### 📏 Standar Kode

#### PHP

```php
<?php
// ✅ Benar - konsisten & jelas
function getUserById(int $id): ?array
{
    if ($id <= 0) {
        return null;
    }
    
    $query = "SELECT * FROM users WHERE userID = :id";
    // ... prepared statement
}

// ❌ Salah - tidak konsisten
function getuser($id){ 
    $q="select * from users where userID=".$id;
}
```

**Aturan PHP:**
- Gunakan `<?php` tag (bukan `<?`)
- Selalu gunakan **prepared statements** untuk query database
- Naming: `camelCase` untuk fungsi, `snake_case` untuk variabel
- Komentar untuk logic yang kompleks
- Indentasi: 4 spasi (bukan tab)

#### JavaScript

```javascript
// ✅ Benar
function validateLevelData(data) {
    if (!data.levelName || data.levelName.length > 40) {
        return { valid: false, error: 'Invalid level name' };
    }
    return { valid: true };
}

// ❌ Salah
function validate(d){
if(!d.n) return false;
}
```

#### HTML

```html
<!-- ✅ Benar - semantic & terstruktur -->
<main class="dashboard">
    <section class="level-list">
        <h2>Recent Levels</h2>
        <div class="level-card">...</div>
    </section>
</main>

<!-- ❌ Salah - semrawut -->
<div class="div1">
    <div class="div2"><p>Recent</p></div>
</div>
```

#### SQL

```sql
-- ✅ Benar - aman & terorganisir
SELECT u.userID, u.userName, l.levelID, l.levelName
FROM users u
INNER JOIN levels l ON u.userID = l.extID
WHERE l.levelID = :levelId
LIMIT 1;

-- ❌ Salah - raw query tanpa parameter
SELECT * FROM users WHERE name = '$name';
```

---

### 📝 Standar Commit

Gunakan format **Conventional Commits**:

```
<tipe>: <deskripsi singkat>

<tipe> yang valid:
  feat     → Fitur baru
  fix      → Perbaikan bug
  docs     → Perubahan dokumentasi
  style    → Formatting (tidak ubah logic)
  refactor → Refactor kode
  test     → Menambah/mengubah test
  chore    → Maintenance, dependencies, dll
```

**Contoh:**
```
feat: tambah fitur search di dashboard
fix: perbaiki crash saat upload song >10MB
docs: update panduan setup database
style: format ulang css dashboard
fix(login): perbaiki redirect loop di halaman login
refactor(db): optimasi query user leaderboard
```

---

### 🔀 Cara Membuat Pull Request

#### Checklist Sebelum PR

```
✅ Sudah fork & buat branch terpisah
✅ Tidak ada conflict dengan main branch
✅ Kode mengikuti standar di atas
✅ Tidak ada kredensial/password di kode
✅ Sudah ditest di local
✅ Commit message mengikuti format
✅ PR description diisi dengan jelas
```

#### Format PR Title

```
[<tipe>] <deskripsi>

Contoh:
[feat] Tambah halaman leaderboard di dashboard
[fix] Perbaiki song upload gagal di Android
[docs] Tambah panduan kontribusi Bahasa Indonesia
```

#### Template PR Description

```markdown
## 📝 Deskripsi
Jelaskan apa yang berubah dan kenapa.

## 🔄 Perubahan
- Detail perubahan 1
- Detail perubahan 2

## 📸 Screenshot (jika ada)
Taruh screenshot di sini

## ✅ Checklist
- [ ] Sudah ditest
- [ ] Tidak ada conflict
- [ ] Mengikuti standar kode

## 🔗 Terkait Issue
Closes #nomor_issue
```

#### Yang Akan Di-review

- **Kualitas kode** — rapi, konsisten, aman
- **Logic** — tidak ada bug yang jelas
- **Security** — tidak ada vulnerability
- **Performance** — tidak ada query berat yang tidak perlu
- **Dokumentasi** — perubahan besar perlu di-dokumentasi

> ⏳ **Review bisa memakan waktu 1-7 hari.** Kami volunteer, bukan full-time dev. Sabar ya!

---

### 🐛 Cara Melaporkan Bug

#### Sebelum Melaporkan

```
1. Cek apakah sudah ada issue yang sama (search dulu!)
2. Coba reproduce bug-nya lagi
3. Pastikan kamu pakai versi terbaru
```

#### Template Laporan Bug

```markdown
## 🐛 Deskripsi Bug
Jelaskan singkat apa yang salah.

## 📋 Langkah Reproduce
1. Buka halaman X
2. Klik tombol Y
3. Isi form dengan Z
4. Klik submit → crash

## ✅ Yang Diharapkan
Seharusnya terjadi...

## ❌ Yang Terjadi
Malah terjadi...

## 📱 Environment
- Server: XAMPP / Hosting / dll
- PHP Version: 8.x
- Browser: Chrome/Firefox
- GDIPS Version: 2.1.3
- Device: PC/Android/iOS

## 📸 Screenshot/Log
Taruh error log atau screenshot di sini

## 📎 Info Tambahan
Ada hal lain yang relevan?
```

#### Label Bug

Kami akan memberi label:
- `bug` — bug terkonfirmasi
- `critical` — bug parah (crash, data loss)
- `minor` — bug kecil (typo, visual)
- `wontfix` — tidak akan diperbaiki (dengan alasan)
- `duplicate` — sudah pernah dilaporkan

---

### 💡 Cara Mengusulkan Fitur

#### Template Usulan Fitur

```markdown
## 💡 Deskripsi Fitur
Jelaskan fitur yang kamu inginkan.

## 🎯 Tujuan
Kenapa fitur ini dibutuhkan? Masalah apa yang diselesaikan?

## 📐 Contoh Implementasi (opsional)
Gambar, mockup, atau pseudocode

## 🔄 Alternatif
Ada cara lain untuk mencapai tujuan yang sama?

## 📊 Dampak
- Pengguna: ...
- Performa: ...
- Keamanan: ...
```

#### Label Fitur

- `enhancement` — usulan fitur
- `discussion` — perlu diskusi dulu
- `accepted` — disetujui, menunggu implementasi
- `planned` — sudah ada di roadmap
- `rejected` — tidak sesuai visi project (dengan alasan)

---

### 🏷 Label Issue Reference

| Label | Arti |
|-------|------|
| `good first issue` | Cocok untuk pemula |
| `help wanted` | Butuh bantuan |
| `priority: high` | Prioritas tinggi |
| `priority: low` | Prioritas rendah |
| `area: frontend` | Terkait dashboard/UI |
| `area: backend` | Terkait server/database |
| `area: security` | Terkait keamanan |
| `area: docs` | Terkait dokumentasi |

---

## English

### 📋 Table of Contents

- [Basic Rules](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-basic-rules)
- [How to Contribute](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-how-to-contribute-1)
- [Development Setup](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-development-setup)
- [Code Standards](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-code-standards)
- [Pull Request Process](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-pull-request-process)
- [Bug Reports](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-bug-reports)
- [Feature Requests](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-feature-requests)

---

### 📜 Basic Rules

> **Read this first before anything.**

1. **Respect everyone** — no toxicity, racism, or bullying
2. **Communicate clearly** — explain problems well, be patient with reviews
3. **Don't copy-paste blindly** — we're here to learn
4. **Mistakes are okay** — bugs happen, what matters is fixing them
5. **Ask when confused** — better to ask than to guess

---

### 🛠 How to Contribute

```
Choose your path:

┌─────────────────────────────────────────────────┐
│                                                 │
│   💻  Code           →  Fix bugs / new features │
│   🐛  Bug Report     →  Report issues           │
│   💡  Ideas          →  Suggest features        │
│   📝  Documentation  →  Write/edit docs         │
│   🎨  Design         →  UI/UX, assets           │
│   🌐  Translation    →  Translate docs/UI       │
│   ⭐  Support        →  Star & share repo       │
│                                                 │
└─────────────────────────────────────────────────┘
```

#### 💻 Code Contribution

1. **Find issues labeled `good first issue`** or `help wanted`**
2. **Comment on the issue**: "I'd like to work on this" (to avoid duplicates)
3. **Fork this repo**
4. **Create a new branch** with a clear name:
   ```bash
   git checkout -b fix/login-crash
   git checkout -b feat/song-upload
   git checkout -b docs/contributing-guide
   ```
5. **Make your changes**
6. **Commit with clear messages** (see [Commit Standards](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-commit-standards))
7. **Push to your fork**
8. **Open a Pull Request**

#### 🐛 Bug Reports

See [Bug Reports](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-bug-reports) section below.

#### 💡 Feature Requests

See [Feature Requests](https://github.com/flessan/GDIPS/blob/main/CONTRIBUTING.md/#-feature-requests) section below.

#### 📝 Documentation

- Note typos, confusing sentences, or missing info
- Open a PR directly or create an issue labeled `documentation`
- Any language is fine (Indonesian/English), as long as it's clear

#### 🎨 Design & Assets

- Open an issue with the `design` label
- Include a preview/image of your proposal
- Format: PNG/SVG for icons, Figma link for layouts

#### 🌐 Translation

- Check which files haven't been translated yet
- Create a PR with filename format: `filename.en.md` (English)
- Don't translate literally — adapt to context

---

### 🖥 Development Setup

#### Prerequisites

```
✅ PHP 7.4+ (8.0+ recommended)
✅ Web Server (Apache/XAMPP/Nginx)
✅ MySQL / MariaDB
✅ Git
✅ Text Editor (VS Code recommended)
✅ Discord account (for communication)
```

#### Setup Steps

```bash
# 1. Fork & Clone the repo
git clone https://github.com/YOU/GDIPS.git
cd GDIPS

# 2. Create a new branch
git checkout -b your-feature

# 3. Setup database
# Import gdips.sql into your MySQL
# Edit database connection config

# 4. Run on local server
# Point your web server to the project folder

# 5. Start coding!
```

#### Main Config File

```php
// Adjust to your environment
define('DB_HOST', 'localhost');
define('DB_NAME', 'gdips_db');
define('DB_USER', 'root');
define('DB_PASS', '');
```

> ⚠️ **Never push real passwords or credentials!**

---

### 📏 Code Standards

#### PHP

```php
<?php
// ✅ Good - consistent & clear
function getUserById(int $id): ?array
{
    if ($id <= 0) {
        return null;
    }
    
    $query = "SELECT * FROM users WHERE userID = :id";
    // ... prepared statement
}

// ❌ Bad - inconsistent
function getuser($id){ 
    $q="select * from users where userID=".$id;
}
```

**PHP Rules:**
- Use `<?php` tags (not `<?`)
- Always use **prepared statements** for database queries
- Naming: `camelCase` for functions, `snake_case` for variables
- Comment complex logic
- Indentation: 4 spaces (not tabs)

#### JavaScript

```javascript
// ✅ Good
function validateLevelData(data) {
    if (!data.levelName || data.levelName.length > 40) {
        return { valid: false, error: 'Invalid level name' };
    }
    return { valid: true };
}

// ❌ Bad
function validate(d){
if(!d.n) return false;
}
```

#### SQL

```sql
-- ✅ Good - safe & organized
SELECT u.userID, u.userName, l.levelID, l.levelName
FROM users u
INNER JOIN levels l ON u.userID = l.extID
WHERE l.levelID = :levelId
LIMIT 1;

-- ❌ Bad - raw query without parameters
SELECT * FROM users WHERE name = '$name';
```

---

### 📝 Commit Standards

Use **Conventional Commits** format:

```
<type>: <short description>

Valid types:
  feat     → New feature
  fix      → Bug fix
  docs     → Documentation change
  style    → Formatting (no logic change)
  refactor → Code refactoring
  test     → Adding/modifying tests
  chore    → Maintenance, dependencies, etc.
```

**Examples:**
```
feat: add search feature to dashboard
fix: fix crash when uploading songs >10MB
docs: update database setup guide
style: reformat dashboard CSS
fix(login): fix redirect loop on login page
refactor(db): optimize user leaderboard query
```

---

### 🔀 Pull Request Process

#### Pre-PR Checklist

```
✅ Forked & created a separate branch
✅ No conflicts with main branch
✅ Code follows the standards above
✅ No credentials/passwords in code
✅ Tested locally
✅ Commit messages follow format
✅ PR description is filled in clearly
```

#### PR Title Format

```
[<type>] <description>

Examples:
[feat] Add leaderboard page to dashboard
[fix] Fix song upload failure on Android
[docs] Add Indonesian contribution guide
```

#### PR Description Template

```markdown
## 📝 Description
Explain what changed and why.

## 🔄 Changes
- Change detail 1
- Change detail 2

## 📸 Screenshots (if any)
Place screenshots here

## ✅ Checklist
- [ ] Tested
- [ ] No conflicts
- [ ] Follows code standards

## 🔗 Related Issue
Closes #issue_number
```

#### What Gets Reviewed

- **Code quality** — clean, consistent, safe
- **Logic** — no obvious bugs
- **Security** — no vulnerabilities
- **Performance** — no unnecessary heavy queries
- **Documentation** — major changes should be documented

> ⏳ **Reviews may take 1-7 days.** We're volunteers, not full-time devs. Please be patient!

---

### 🐛 Bug Reports

#### Before Reporting

```
1. Check if a similar issue already exists (search first!)
2. Try to reproduce the bug again
3. Make sure you're on the latest version
```

#### Bug Report Template

```markdown
## 🐛 Bug Description
Briefly explain what's wrong.

## 📋 Steps to Reproduce
1. Open page X
2. Click button Y
3. Fill form with Z
4. Click submit → crash

## ✅ Expected Behavior
What should happen...

## ❌ Actual Behavior
What actually happens...

## 📱 Environment
- Server: XAMPP / Hosting / etc
- PHP Version: 8.x
- Browser: Chrome/Firefox
- GDIPS Version: 2.1.3
- Device: PC/Android/iOS

## 📸 Screenshots/Logs
Place error logs or screenshots here

## 📎 Additional Info
Anything else relevant?
```

---

### 💡 Feature Requests

#### Feature Request Template

```markdown
## 💡 Feature Description
Describe the feature you want.

## 🎯 Goal
Why is this needed? What problem does it solve?

## 📐 Implementation Example (optional)
Image, mockup, or pseudocode

## 🔄 Alternatives
Other ways to achieve the same goal?

## 📊 Impact
- Users: ...
- Performance: ...
- Security: ...
```

---

### 🏷 Issue Label Reference

| Label | Meaning |
|-------|---------|
| `good first issue` | Good for beginners |
| `help wanted` | Needs help |
| `priority: high` | High priority |
| `priority: low` | Low priority |
| `area: frontend` | Related to dashboard/UI |
| `area: backend` | Related to server/database |
| `area: security` | Related to security |
| `area: docs` | Related to documentation |

---

<div align="center">

## 💬 Pertanyaan?

Jangan ragu untuk bertanya di:

[![Discord](https://img.shields.io/badge/Discord-Ask_Here-5865F2?logo=discord)](https://discord.gg/YyeZ2Sxjgf)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Ask_Here-25D366?logo=whatsapp)](https://chat.whatsapp.com/Fmh5DoSjbWkBje0ab3RAEF)

---

> *"Tidak ada kontribusi yang terlalu kecil. Satu typo fix sudah berarti."*

**Selamat berkontribusi! 🎉**

![Divider](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

</div>

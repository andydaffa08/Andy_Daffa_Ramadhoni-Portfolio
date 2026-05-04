# Execution — Andy Daffa Ramadhoni

## Step 1: Membuat Struktur Dasar Semantic HTML5

### Prompt
Sebagai Senior Front-end Developer, buatkan struktur dasar index.html untuk portfolio satu halaman saya. Gunakan tag Semantic HTML5 lengkap seperti <header>, <nav>, <main>, <section>, dan <footer>. Portfolio ini harus mencakup bagian Hero, Dual-Skill Matrix (Hardware & UI/UX), Selected Projects, The Lab (Hardware Gallery), dan Contact. Ikuti batasan: jangan gunakan tag <div> jika ada tag semantik yang tersedia

### RTCC-O Check
- R: ✅
- T: ✅
- C: ✅
- C: ✅
- O: ✅

### AI Response
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Andy Daffa Ramadhoni | Hardware & UI/UX Specialist</title>
    <meta name="description" content="Portfolio Andy Daffa Ramadhoni - Spesialis Hardware Troubleshooting dan UI/UX Designer.">
</head>
<body>

    <!-- Header & Navigation -->
    <header>
        <nav aria-label="Main Navigation">
            <ul>
                <li><a href="#hero">Beranda</a></li>
                <li><a href="#matrix">Keahlian</a></li>
                <li><a href="#projects">Proyek</a></li>
                <li><a href="#lab">The Lab</a></li>
                <li><a href="#contact">Kontak</a></li>
            </ul>
        </nav>
    </header>

    <!-- Main Content Area -->
    <main>

        <!-- 1. Hero Section -->
        <section id="hero">
            <header>
                <h1>Andy Daffa Ramadhoni</h1>
                <p>I fix the hardware, I design the experience.</p>
            </header>
            <p>Menjembatani pemahaman mendalam tentang arsitektur perangkat keras dengan desain antarmuka pengguna yang intuitif.</p>
            <a href="#projects" role="button">Lihat Pekerjaan Saya</a>
        </section>

        <!-- 2. Dual-Skill Matrix Section -->
        <section id="matrix">
            <h2>Keahlian Utama</h2>
            
            <article>
                <h3>UI/UX Design</h3>
                <p>Merancang antarmuka mobile-first yang efisien dan berpusat pada pengguna.</p>
                <ul>
                    <li>User Research</li>
                    <li>Wireframing & Prototyping</li>
                    <li>Interaction Design</li>
                </ul>
            </article>

            <article>
                <h3>Hardware & PC Maintenance</h3>
                <p>Pemecahan masalah teknis, manajemen daya, dan optimalisasi perangkat keras keras.</p>
                <ul>
                    <li>Troubleshooting Laptop/Mobile</li>
                    <li>Hardware Upgrades</li>
                    <li>System Optimization</li>
                </ul>
            </article>
        </section>

        <!-- 3. Selected Projects Section -->
        <section id="projects">
            <h2>Proyek Pilihan</h2>
            
            <article>
                <header>
                    <h3>Sistem Informasi Rumah Sakit</h3>
                    <p>UI/UX Designer</p>
                </header>
                <figure>
                    <img src="project1-thumbnail.jpg" alt="Mockup aplikasi sistem informasi rumah sakit">
                    <figcaption>Desain ulang antarmuka untuk staf medis.</figcaption>
                </figure>
                <p>Meningkatkan efisiensi input data pasien melalui perbaikan arsitektur informasi dan layout mobile.</p>
            </article>

            <article>
                <header>
                    <h3>Mobile JKN Transition Flow</h3>
                    <p>UX Case Study</p>
                </header>
                <figure>
                    <img src="project2-thumbnail.jpg" alt="Alur transisi segmen di Mobile JKN">
                    <figcaption>Analisis dan perbaikan alur pengguna.</figcaption>
                </figure>
                <p>Menyederhanakan proses perubahan status asuransi kesehatan dengan mengurangi langkah kognitif pengguna.</p>
            </article>
        </section>

        <!-- 4. The Lab (Hardware Gallery) Section -->
        <section id="lab">
            <h2>The Lab</h2>
            <p>Ruang kerja nyata tempat saya membedah dan mengoptimalkan perangkat.</p>
            
            <figure>
                <img src="lab-ram-upgrade.jpg" alt="Proses upgrade RAM pada laptop Acer">
                <figcaption>Presisi dalam instalasi komponen fisik.</figcaption>
            </figure>
            
            <figure>
                <img src="lab-battery-reset.jpg" alt="Pemecahan masalah baterai internal laptop">
                <figcaption>Troubleshooting tingkat sirkuit dan manajemen daya.</figcaption>
            </figure>
        </section>

        <!-- 5. Contact Section -->
        <section id="contact">
            <h2>Mari Terhubung</h2>
            <p>Terbuka untuk diskusi mengenai desain produk atau sekadar obrolan tentang optimasi perangkat.</p>
            
            <address>
                <p>Email: <a href="mailto:andy.daffa@email.com">andy.daffa@email.com</a></p>
                <p>Lokasi: Serang, Banten</p>
            </address>

            <!-- Form Kontak Semantik -->
            <form action="/submit-form" method="POST">
                <fieldset>
                    <legend>Kirim Pesan</legend>
                    
                    <label for="name">Nama:</label>
                    <input type="text" id="name" name="name" required>
                    
                    <label for="message">Pesan:</label>
                    <textarea id="message" name="message" rows="4" required></textarea>
                    
                    <button type="submit">Kirim Pesan</button>
                </fieldset>
            </form>
        </section>

    </main>

    <!-- Footer -->
    <footer>
        <small>&copy; 2026 Andy Daffa Ramadhoni. Dibuat dengan HTML5 Semantik.</small>
    </footer>

</body>
</html>

### Review
- [✅] Sesuai constraints?
- [✅] Format sesuai?
- [✅] Bisa dipahami?
- Changes: membuat class text bold pada tag p pada section id  “matrix” agar huruf terlihat tebal

---

## Step 2: Styling Dasar & Layout Mobile-First (Cyber Circuit)

### Prompt
"Sekarang, buatkan file style.css terpisah menggunakan pendekatan mobile-first. Terapkan palet warna 'Cyber Circuit' (Deep Navy, Teal, dan Ghost White) serta tipografi 'Plus Jakarta Sans' dan 'Inter'. Pastikan layout menggunakan sistem flexbox atau grid yang rapi dan tidak ada horizontal scroll pada layar HP

### RTCC-O Check
- R: ✅
- T: ✅
- C: ✅
- C: ✅
- O: ✅

### AI Response

/* --- RESET & VARIABLES --- */
:root {
    --deep-navy: #0F172A;
    --teal: #2DD4BF;
    --ghost-white: #F8FAFC;
    --slate: #475569;
    
    --font-heading: 'Plus Jakarta Sans', sans-serif;
    --font-body: 'Inter', sans-serif;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    background-color: var(--ghost-white);
    color: var(--deep-navy);
    font-family: var(--font-body);
    line-height: 1.6;
    overflow-x: hidden; /* Mencegah horizontal scroll di level body */
}

/* --- TYPOGRAPHY --- */
h1, h2, h3 {
    font-family: var(--font-heading);
    color: var(--deep-navy);
    line-height: 1.2;
    margin-bottom: 1rem;
}

a {
    text-decoration: none;
    color: var(--teal);
    transition: 0.3s ease;
}

/* --- LAYOUT UTILITIES --- */
section {
    padding: 4rem 1.5rem;
    max-width: 100%; /* Menjamin tidak melebar keluar viewport */
}

/* --- HEADER & NAV --- */
header {
    background-color: var(--deep-navy);
    padding: 1rem;
    position: sticky;
    top: 0;
    z-index: 1000;
}

nav ul {
    display: flex;
    justify-content: space-around;
    list-style: none;
}

nav a {
    color: var(--ghost-white);
    font-size: 0.85rem;
    font-weight: 500;
}

/* --- HERO SECTION --- */
#hero {
    background-color: var(--deep-navy);
    color: var(--ghost-white);
    text-align: center;
    min-height: 80vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

#hero h1 {
    color: var(--teal);
    font-size: 2.5rem;
}

#hero [role="button"] {
    background-color: var(--teal);
    color: var(--deep-navy);
    padding: 0.8rem 1.5rem;
    border-radius: 8px;
    font-weight: 700;
    margin-top: 1.5rem;
}

/* --- MATRIX (FLEXBOX) --- */
#matrix {
    display: flex;
    flex-direction: column;
    gap: 2rem;
}

#matrix article {
    background: white;
    padding: 2rem;
    border-left: 4px solid var(--teal);
    box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1);
}

/* --- SELECTED PROJECTS (GRID) --- */
#projects {
    display: grid;
    grid-template-columns: 1fr; /* Satu kolom untuk mobile */
    gap: 2.5rem;
}

#projects article {
    display: flex;
    flex-direction: column;
}

#projects img {
    width: 100%;
    height: auto;
    border-radius: 12px;
    object-fit: cover;
}

/* --- THE LAB (GALLERY GRID) --- */
#lab {
    background-color: #f1f5f9;
}

#lab figure {
    margin-bottom: 2rem;
}

#lab img {
    width: 100%;
    border-radius: 8px;
    filter: grayscale(20%);
}

/* --- CONTACT FORM --- */
form {
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

fieldset {
    border: 1px solid #cbd5e1;
    padding: 1.5rem;
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

input, textarea {
    width: 100%;
    padding: 0.8rem;
    border: 1px solid #cbd5e1;
    border-radius: 4px;
    font-family: var(--font-body);
}

button {
    background-color: var(--deep-navy);
    color: var(--teal);
    padding: 1rem;
    border: none;
    font-weight: bold;
    cursor: pointer;
}

/* --- FOOTER --- */
footer {
    text-align: center;
    padding: 2rem;
    background: var(--deep-navy);
    color: var(--ghost-white);
}

/* --- MEDIA QUERIES (DESKTOP) --- */
@media (min-width: 768px) {
    #matrix {
        flex-direction: row;
    }
    
    #projects {
        grid-template-columns: repeat(2, 1fr);
    }
    
    #hero h1 {
        font-size: 4rem;
    }
}

### Review
- [✅] Sesuai constraints?
- [✅] Format sesuai?
- [✅] Bisa dipahami?
- Changes: menambahkan media queries agar konten atau gambar terlihat sejajar

---

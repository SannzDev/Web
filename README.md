
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MY BIODATA</title>

<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;600;800&family=Poppins:wght@300;400;500&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

:root{
    --primary:#00e5ff;
    --secondary:#8a2be2;
    --dark:#070b14;
    --glass:rgba(255,255,255,0.08);
}

body{
    background:var(--dark);
    color:white;
    font-family:'Poppins',sans-serif;
    overflow-x:hidden;
}

/* Animated Background */
body::before{
    content:"";
    position:fixed;
    inset:0;
    background:
    radial-gradient(circle at 20% 30%, rgba(0,229,255,.15), transparent 30%),
    radial-gradient(circle at 80% 70%, rgba(138,43,226,.15), transparent 30%);
    animation: moveBg 8s infinite alternate;
    z-index:-2;
}

@keyframes moveBg{
    from{
        transform:scale(1);
    }
    to{
        transform:scale(1.2);
    }
}

/* Navbar */
nav{
    position:fixed;
    width:100%;
    top:0;
    padding:20px 8%;
    display:flex;
    justify-content:space-between;
    align-items:center;
    backdrop-filter:blur(20px);
    background:rgba(0,0,0,0.25);
    z-index:1000;
}

.logo{
    font-family:'Orbitron',sans-serif;
    font-size:1.5rem;
    color:var(--primary);
    font-weight:800;
}

nav ul{
    display:flex;
    gap:30px;
    list-style:none;
}

nav a{
    text-decoration:none;
    color:white;
    transition:.3s;
}

nav a:hover{
    color:var(--primary);
}

/* Hero */
.hero{
    min-height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    padding:100px 8%;
}

.hero-content{
    text-align:center;
    max-width:800px;
}

.hero h1{
    font-family:'Orbitron',sans-serif;
    font-size:4rem;
    margin-bottom:20px;
    background:linear-gradient(90deg,var(--primary),#fff,var(--secondary));
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
}

.hero p{
    font-size:1.1rem;
    opacity:.8;
    margin-bottom:30px;
}

.btn{
    display:inline-block;
    padding:15px 35px;
    border:2px solid var(--primary);
    border-radius:50px;
    color:white;
    text-decoration:none;
    transition:.3s;
    box-shadow:0 0 20px var(--primary);
}

.btn:hover{
    background:var(--primary);
    color:black;
}

/* Sections */
section{
    padding:100px 8%;
}

.section-title{
    text-align:center;
    font-size:2.5rem;
    font-family:'Orbitron',sans-serif;
    margin-bottom:50px;
    color:var(--primary);
}

/* About */
.about-card{
    background:var(--glass);
    backdrop-filter:blur(20px);
    border:1px solid rgba(255,255,255,.1);
    border-radius:20px;
    padding:40px;
    text-align:center;
}

/* Projects */
.projects{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:25px;
}

.project{
    background:var(--glass);
    backdrop-filter:blur(15px);
    border-radius:20px;
    padding:25px;
    transition:.4s;
    border:1px solid rgba(255,255,255,.1);
}

.project:hover{
    transform:translateY(-10px);
    box-shadow:0 0 30px rgba(0,229,255,.4);
}

.project h3{
    color:var(--primary);
    margin-bottom:10px;
}

/* Skills */
.skills{
    display:flex;
    flex-wrap:wrap;
    gap:15px;
    justify-content:center;
}

.skill{
    padding:12px 20px;
    border:1px solid var(--primary);
    border-radius:50px;
    background:rgba(0,229,255,.08);
}

/* Contact */
.contact{
    text-align:center;
}

.contact a{
    color:var(--primary);
    text-decoration:none;
}

/* Footer */
footer{
    text-align:center;
    padding:30px;
    border-top:1px solid rgba(255,255,255,.1);
    opacity:.7;
}

/* Floating Glow */
.glow{
    position:absolute;
    width:300px;
    height:300px;
    border-radius:50%;
    background:var(--primary);
    filter:blur(150px);
    opacity:.15;
    animation:float 8s infinite alternate;
}

.glow2{
    background:var(--secondary);
    right:0;
    bottom:0;
}

@keyframes float{
    from{
        transform:translateY(0);
    }
    to{
        transform:translateY(-100px);
    }
}

@media(max-width:768px){
    .hero h1{
        font-size:2.5rem;
    }

    nav ul{
        gap:15px;
        font-size:.9rem;
    }
}
</style>
</head>
<body>

<div class="glow"></div>
<div class="glow glow2"></div>

<nav>
    <div class="logo">PORTFOLIO</div>

    <ul>
        <li><a href="#about">Tentang</a></li>
        <li><a href="#projects">Project</a></li>
        <li><a href="#skills">Skill</a></li>
        <li><a href="#contact">Kontak</a></li>
    </ul>
</nav>

<section class="hero">
    <div class="hero-content">
        <h1>HALLO, SAYA SannzDev</h1>
        <p>
            Frontend Developer & UI/UX Designer yang fokus
            membangun pengalaman digital modern dengan
            teknologi masa depan.
        </p>

        <a href="#projects" class="btn">Lihat Project</a>
    </div>
</section>

<section id="about">
    <h2 class="section-title">Tentang Saya</h2>

    <div class="about-card">
        <p>
            salam semuanya nama saya Ilham umur 14 tahun seorang web design open jasa design web saya juga seorang web operator, game developer dan seorang IT master, asli jaksel dan seorang peminat manhwa.
        </p>
    </div>
</section>

<section id="projects">
    <h2 class="section-title">Project</h2>

    <div class="projects">

        <div class="project">
            <h3>WEB DESIGN</h3>
            <p>Web Design berbasis html dengan aneka tema mulai dari datar, colorful,futuristik, elegen dan modern theme.</p>
        </div>

        <div class="project">
            <h3>GAME DEVELOPER</h3>
            <p>Game developer, membuqt game yang menarik sesuai kreativitas dan bisa membuat game yang menyesuaikan dengan minat dan imajinasi.</p>
        </div>

        <div class="project">
            <h3>LOCK HANDPHONE</h3>
            <p>pelopor aplikasi LOCK HANDPHONE yang bisa membuat kamu mengunci hp seseorang yang hanya bisa di buka dengan kunci yang kamu pegang.</p>
        </div>

    </div>
</section>

<section id="skills">
    <h2 class="section-title">Skills</h2>

    <div class="skills">
        <div class="skill">HTML5</div>
        <div class="skill">CSS3</div>
        <div class="skill">JavaScript</div>
        <div class="skill">React</div>
        <div class="skill">Node.js</div>
        <div class="skill">UI/UX</div>
        <div class="skill">Figma</div>
        <div class="skill">AI Integration</div>
    </div>
</section>

<section id="contact">
    <h2 class="section-title">Kontak</h2>

    <div class="contact">
        <p>Email: emailanda@example.com</p>
        <p>Instagram: @username</p>
        <p>GitHub: github.com/username</p>
    </div>
</section>

<footer>
    © 2026 Portfolio Futuristik | Dibuat dengan HTML, CSS & JavaScript
</footer>

<script>

// Efek muncul saat scroll
const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
        if(entry.isIntersecting){
            entry.target.style.opacity = "1";
            entry.target.style.transform = "translateY(0)";
        }
    });
});

document.querySelectorAll('.project, .about-card, .skill').forEach(el => {
    el.style.opacity = "0";
    el.style.transform = "translateY(30px)";
    el.style.transition = "0.8s";
    observer.observe(el);
});

</script>

</body>
</html>

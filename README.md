<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>KAIMA | Intelligent Software Solutions</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>
:root{
    --primary:#4f46e5;
    --secondary:#8b5cf6;
    --dark:#081122;
    --dark2:#111827;
    --light:#f8fafc;
    --text:#334155;
    --gradient:linear-gradient(135deg,#2563eb,#8b5cf6);
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Inter',sans-serif;
}

html{
    scroll-behavior:smooth;
}

body{
    background:#fff;
    color:var(--text);
    overflow-x:hidden;
}

.container{
    width:90%;
    max-width:1300px;
    margin:auto;
}

/* ================= HEADER ================= */

header{
    position:fixed;
    width:100%;
    top:0;
    z-index:1000;
    background:rgba(8,17,34,.95);
    backdrop-filter:blur(12px);
    border-bottom:1px solid rgba(255,255,255,.08);
}

.navbar{
    display:flex;
    justify-content:space-between;
    align-items:center;
    height:80px;
}

.logo{
    font-size:2rem;
    font-weight:800;
    background:linear-gradient(90deg,#3b82f6,#8b5cf6);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
}

.nav-links{
    display:flex;
    gap:35px;
}

.nav-links a{
    text-decoration:none;
    color:white;
    font-weight:500;
    transition:.35s;
    position:relative;
}

.nav-links a::after{
    content:'';
    position:absolute;
    left:0;
    bottom:-6px;
    width:0;
    height:2px;
    background:#8b5cf6;
    transition:.35s;
}

.nav-links a:hover{
    color:#c4b5fd;
    text-shadow:0 0 15px #8b5cf6;
}

.nav-links a:hover::after{
    width:100%;
}

/* ================= HERO ================= */

.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    background:linear-gradient(135deg,#1d4ed8,#6d28d9);
    position:relative;
    overflow:hidden;
}

.hero-content{
    position:relative;
    z-index:2;
    color:white;
    text-align:center;
}

.hero h1{
    font-size:4rem;
    line-height:1.1;
    margin-bottom:20px;
}

.hero p{
    max-width:700px;
    margin:auto;
    font-size:1.15rem;
    opacity:.9;
}

.hero-buttons{
    margin-top:35px;
    display:flex;
    justify-content:center;
    gap:20px;
    flex-wrap:wrap;
}

.btn{
    padding:16px 34px;
    border-radius:50px;
    text-decoration:none;
    font-weight:600;
    transition:.4s;
}

.btn-primary{
    background:#8b5cf6;
    color:white;
}

.btn-primary:hover{
    transform:translateY(-4px);
    box-shadow:0 15px 35px rgba(139,92,246,.5);
}

.btn-secondary{
    border:2px solid #60a5fa;
    color:white;
}

.btn-secondary:hover{
    background:#60a5fa;
    color:#081122;
}

/* Floating Shapes */

.shape{
    position:absolute;
    border:1px solid rgba(255,255,255,.15);
    backdrop-filter:blur(10px);
    animation:float 12s infinite ease-in-out;
}

.shape1{
    width:180px;
    height:180px;
    border-radius:30px;
    top:15%;
    left:8%;
}

.shape2{
    width:100px;
    height:100px;
    border-radius:50%;
    top:60%;
    right:12%;
    animation-delay:2s;
}

.shape3{
    width:150px;
    height:150px;
    transform:rotate(45deg);
    top:20%;
    right:15%;
    animation-delay:4s;
}

.code{
    position:absolute;
    color:rgba(255,255,255,.15);
    font-weight:700;
    font-size:1.2rem;
    animation:float 15s infinite;
}

.code1{
    top:30%;
    left:15%;
}

.code2{
    top:65%;
    right:20%;
}

@keyframes float{
    0%,100%{
        transform:translateY(0);
    }
    50%{
        transform:translateY(-30px);
    }
}

/* ================= SECTION ================= */

section{
    padding:100px 0;
}

.section-title{
    text-align:center;
    margin-bottom:60px;
}

.section-title h2{
    font-size:2.8rem;
    color:#0f172a;
}

.section-title p{
    color:#64748b;
    margin-top:10px;
}

/* ================= SERVICES ================= */

.services{
    background:#f8fafc;
}

.services-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:30px;
}

.service-card{
    background:white;
    padding:40px;
    border-radius:24px;
    transition:.4s;
    box-shadow:0 10px 30px rgba(59,130,246,.08);
}

.service-card:hover{
    transform:translateY(-10px);
    box-shadow:0 0 35px rgba(59,130,246,.3);
}

.service-icon{
    width:70px;
    height:70px;
    background:rgba(139,92,246,.1);
    color:#8b5cf6;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:2rem;
    border-radius:18px;
    margin-bottom:20px;
}

.service-card h3{
    margin-bottom:15px;
    color:#0f172a;
}

/* ================= ABOUT ================= */

.about{
    background:linear-gradient(135deg,#f3e8ff,#eef2ff);
}

.about-content{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:60px;
    align-items:center;
}

.about-text h2{
    font-size:2.8rem;
    color:#0f172a;
    margin-bottom:20px;
}

.about-text p{
    line-height:1.8;
}

.about-visual{
    position:relative;
    height:400px;
}

.about-box{
    width:100%;
    height:100%;
    border-radius:30px;
    background:linear-gradient(135deg,#2563eb,#8b5cf6);
    box-shadow:0 30px 60px rgba(37,99,235,.3);
    position:relative;
}

.about-box::before{
    content:'';
    position:absolute;
    inset:20px;
    border-radius:20px;
    border:2px solid rgba(255,255,255,.3);
}

/* ================= TESTIMONIALS ================= */

.clients{
    background:#081122;
    color:white;
}

.logo-carousel{
    display:flex;
    gap:30px;
    overflow:hidden;
    white-space:nowrap;
}

.client-logo{
    min-width:220px;
    background:#111827;
    border-radius:20px;
    padding:30px;
    text-align:center;
    color:#94a3b8;
    font-weight:700;
    transition:.4s;
}

.client-logo:hover{
    color:#60a5fa;
    background:linear-gradient(135deg,#2563eb,#8b5cf6);
}

/* ================= FOOTER ================= */

footer{
    background:#2e1065;
    color:white;
    padding:60px 0 30px;
}

.footer-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:40px;
}

.footer-links{
    display:flex;
    flex-direction:column;
    gap:12px;
}

.footer-links a{
    color:#cbd5e1;
    text-decoration:none;
    transition:.3s;
}

.footer-links a:hover{
    color:#60a5fa;
}

.socials{
    display:flex;
    gap:15px;
    margin-top:20px;
}

.socials a{
    width:45px;
    height:45px;
    border-radius:50%;
    display:flex;
    align-items:center;
    justify-content:center;
    background:rgba(255,255,255,.08);
    color:white;
    text-decoration:none;
    transition:.3s;
}

.socials a:hover{
    background:#3b82f6;
    transform:translateY(-5px);
}

.copyright{
    text-align:center;
    margin-top:50px;
    border-top:1px solid rgba(255,255,255,.1);
    padding-top:20px;
    color:#cbd5e1;
}

/* ================= RESPONSIVE ================= */

@media(max-width:900px){

    .hero h1{
        font-size:2.8rem;
    }

    .about-content{
        grid-template-columns:1fr;
    }

    .nav-links{
        display:none;
    }
}

@media(max-width:600px){

    .hero h1{
        font-size:2.2rem;
    }

    .section-title h2{
        font-size:2rem;
    }
}
</style>
</head>
<body>

<header>
    <div class="container navbar">
        <div class="logo">KAIMA</div>

        <nav class="nav-links">
            <a href="#">Home</a>
            <a href="#services">Services</a>
            <a href="#about">About</a>
            <a href="#clients">Clients</a>
            <a href="#contact">Contact</a>
        </nav>
    </div>
</header>

<section class="hero">
    <div class="shape shape1"></div>
    <div class="shape shape2"></div>
    <div class="shape shape3"></div>

    <div class="code code1">&lt;/AI&gt;</div>
    <div class="code code2">{ Cloud }</div>

    <div class="container hero-content">
        <h1>Building the Future with Intelligent Software</h1>

        <p>
            KAIMA delivers cutting-edge software solutions, AI innovation,
            cloud infrastructure, and scalable digital products that help
            businesses thrive in the modern world.
        </p>

        <div class="hero-buttons">
            <a href="#" class="btn btn-primary">Get Started</a>
            <a href="#" class="btn btn-secondary">Our Services</a>
        </div>
    </div>
</section>

<section class="services" id="services">
    <div class="container">

        <div class="section-title">
            <h2>Our Services</h2>
            <p>Innovative technology solutions built for growth.</p>
        </div>

        <div class="services-grid">

            <div class="service-card">
                <div class="service-icon">🌐</div>
                <h3>Web Development</h3>
                <p>
                    Modern websites and enterprise applications built for
                    performance, security, and scalability.
                </p>
            </div>

            <div class="service-card">
                <div class="service-icon">🤖</div>
                <h3>AI Solutions</h3>
                <p>
                    Intelligent automation, machine learning, and AI-powered
                    experiences that drive efficiency.
                </p>
            </div>

            <div class="service-card">
                <div class="service-icon">☁️</div>
                <h3>Cloud Services</h3>
                <p>
                    Secure cloud infrastructure, deployment pipelines,
                    and enterprise-grade hosting solutions.
                </p>
            </div>

        </div>

    </div>
</section>

<section class="about" id="about">
    <div class="container">

        <div class="about-content">

            <div class="about-text">
                <h2>About KAIMA</h2>

                <p>
                    KAIMA is a forward-thinking software company focused on
                    delivering exceptional digital experiences. We combine
                    advanced engineering, cloud technologies, and artificial
                    intelligence to create solutions that empower organizations
                    to innovate faster and operate smarter.
                </p>
            </div>

            <div class="about-visual">
                <div class="about-box"></div>
            </div>

        </div>

    </div>
</section>

<section class="clients" id="clients">

    <div class="container">

        <div class="section-title">
            <h2 style="color:white;">Trusted By Growing Businesses</h2>
            <p style="color:#94a3b8;">
                Companies that rely on innovation.
            </p>
        </div>

        <div class="logo-carousel">
            <div class="client-logo">TECHCORP</div>
            <div class="client-logo">NEXUS</div>
            <div class="client-logo">SKYCLOUD</div>
            <div class="client-logo">INNOVATE AI</div>
            <div class="client-logo">DIGITAL EDGE</div>
        </div>

    </div>

</section>

<footer id="contact">

    <div class="container">

        <div class="footer-grid">

            <div>
                <h3>KAIMA</h3>
                <p style="margin-top:15px;">
                    Building innovative software solutions for the future.
                </p>
            </div>

            <div class="footer-links">
                <h4>Quick Links</h4>
                <a href="#">Home</a>
                <a href="#">Services</a>
                <a href="#">About</a>
                <a href="#">Contact</a>
            </div>

            <div class="footer-links">
                <h4>Contact</h4>
                <a href="#">hello@kaima.com</a>
                <a href="#">+234 XXX XXX XXXX</a>
                <a href="#">Lagos, Nigeria</a>
            </div>

            <div>
                <h4>Follow Us</h4>

                <div class="socials">
                    <a href="#">X</a>
                    <a href="#">in</a>
                    <a href="#">f</a>
                    <a href="#">ig</a>
                </div>
            </div>

        </div>

        <div class="copyright">
            © 2026 KAIMA Software. All Rights Reserved.
        </div>

    </div>

</footer>

</body>
</html># software-
software 

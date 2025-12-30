<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Frontline | Humanitarian Aid</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;600;700&family=Quicksand:wght@500;700&display=swap" rel="stylesheet">
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">

    <style>
        :root {
            --primary-blue: #00AEEF;
            --primary-pink: #EC6DB0;
            --text-gray: #666;
            --light-bg: #F9FAFB;
            --gradient: linear-gradient(90deg, #00AEEF, #EC6DB0);
        }

        * { box-sizing: border-box; margin: 0; padding: 0; scroll-behavior: smooth; }

        body {
            font-family: 'Quicksand', sans-serif;
            background-color: #ffffff;
            color: var(--text-gray);
            line-height: 1.6;
        }

        h1, h2, h3, .logo, nav a { font-family: 'Fredoka', sans-serif; }

        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 8%;
            background: white;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.02);
        }

        .logo i { font-size: 2.2rem; color: #5D5FEF; }

        nav a {
            text-decoration: none;
            color: #333;
            margin-left: 20px;
            font-weight: 600;
            transition: color 0.3s;
        }
        
        nav a:hover { color: var(--primary-blue); }

        .hero { padding: 60px 8%; text-align: center; background-color: var(--light-bg); }

        .hero-card {
            background: white;
            padding: 60px 40px;
            border-radius: 30px;
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.04);
            max-width: 950px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 4rem;
            background: linear-gradient(90deg, #7A8FFF, #FF839D);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 20px;
        }

        .btn-gradient {
            border: none;
            padding: 16px 35px;
            border-radius: 50px;
            color: white;
            font-family: 'Fredoka', sans-serif;
            font-weight: 600;
            cursor: pointer;
            background: var(--gradient);
            box-shadow: 0 8px 20px rgba(236, 109, 176, 0.2);
            margin: 10px;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
        }

        .btn-gradient:hover { transform: scale(1.05); }

        section { padding: 80px 8%; text-align: center; }

        .section-title { color: var(--primary-blue); font-size: 2.5rem; margin-bottom: 25px; }

        .progress-container {
            background: #F0F0F0;
            height: 30px;
            border-radius: 20px;
            max-width: 600px;
            margin: 20px auto;
            overflow: hidden;
        }
        .progress-bar { width: 0%; height: 100%; background: #E0E0E0; }

        .team-grid { display: flex; gap: 30px; justify-content: center; flex-wrap: wrap; margin-top: 40px;}
        .team-card {
            background: white;
            padding: 40px 25px;
            border-radius: 25px;
            flex: 1;
            min-width: 280px;
            max-width: 320px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
            text-align: left;
        }

        .profile-circle {
            width: 140px; height: 140px; border-radius: 50%;
            border: 5px solid var(--primary-blue); margin: 0 auto 20px;
            overflow: hidden; background: #eee;
        }
        .profile-circle img { width: 100%; height: 100%; object-fit: cover; }

        input, textarea {
            width: 100%; padding: 18px; margin-bottom: 15px;
            border: 2px solid #F0F0F0; border-radius: 15px;
            font-family: 'Quicksand', sans-serif;
            background: #FAFAFA;
        }

        footer { padding: 60px 8%; text-align: center; background: #fff; border-top: 1px solid #eee; }
        
        .social-handle {
            display: block;
            margin-top: 10px;
            font-weight: 700;
            color: #7A8FFF;
            text-decoration: none;
            font-size: 1.2rem;
        }

        .social-icons { margin: 20px 0; font-size: 1.8rem; }
        .social-icons a { margin: 0 15px; color: #7A8FFF; text-decoration: none; transition: 0.3s; }
        .social-icons a:hover { color: var(--primary-pink); }
        
        .footer-info { font-size: 0.9rem; color: #bbb; margin-top: 20px; font-weight: 600; }
    </style>
</head>
<body>

    <header>
        <div class="logo"><i class="fas fa-hand-holding-medical"></i></div>
        <nav>
            <a href="#mission">Mission</a>
            <a href="#team">Team</a>
            <a href="#volunteer">Volunteer</a>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-card">
            <h1>Frontline</h1>
            <p>Aiding people in war-affected regions like Gaza and Ukraine — supplying immediate relief and longer-term support.</p>
            <a href="#mission" class="btn-gradient">Donate Now</a>
            <a href="#volunteer" class="btn-gradient">Join as Volunteer</a>
        </div>
    </section>

    <section id="mission">
        <h2 class="section-title">Our Mission</h2>
        <p style="max-width: 800px; margin: 0 auto 30px;">We aim to raise $25,000 to support families displaced and affected by conflicts. We channel resources through vetted partners and local volunteers to make relief fast and accountable.</p>
        
        <div class="progress-container"><div class="progress-bar"></div></div>
        <p style="font-weight: 700; color: #999;">$0 raised of $25,000 goal</p>

        <h2 class="section-title" style="margin-top: 50px;">Support Our Cause</h2>
        <div>
            <a href="https://www.paypal.com/paypalme/YOUR_HANDLE" target="_blank" class="btn-gradient">Donate via PayPal</a>
            <a href="https://www.gofundme.com/f/YOUR_CAMPAIGN" target="_blank" class="btn-gradient">Donate via GoFundMe</a>
            <a href="https://venmo.com/u/YOUR_HANDLE" target="_blank" class="btn-gradient">Donate via Venmo</a>
        </div>
    </section>

    <section id="team" style="background: var(--light-bg);">
        <h2 class="section-title">Meet Our Team</h2>
        <div class="team-grid">
            <div class="team-card">
                <div class="profile-circle"><img src="https://via.placeholder.com/150" alt="Priya"></div>
                <h3>Priya Maydipalle</h3>
                <p><strong>President</strong></p>
                <p class="bio" style="font-size: 0.9rem;">Rising senior at Westborough High School. Dedicated to rebuilding lives through small acts of kindness.</p>
            </div>
            <div class="team-card">
                <div class="profile-circle"><img src="https://via.placeholder.com/150" alt="Hasini"></div>
                <h3>Hasini Garrepalli</h3>
                <p><strong>Treasurer</strong></p>
                <p class="bio" style="font-size: 0.9rem;">Rising junior at Franklin High School. Believes uplifting others is the most valuable use of time.</p>
            </div>
            <div class="team-card">
                <div class="profile-circle"><img src="https://via.placeholder.com/150" alt="Yashhu"></div>
                <h3>Yashhu Kukula</h3>
                <p><strong>Secretary</strong></p>
                <p class="bio" style="font-size: 0.9rem;">Rising junior at Ashland High School. Passionate about art and music, believing compassion has the power to heal.</p>
            </div>
        </div>
    </section>

    <section id="volunteer">
        <h2 class="section-title">Volunteer With Us</h2>
        <form action="https://formspree.io/f/YOUR_FORMSPREE_ID" method="POST" style="max-width: 600px; margin: 0 auto;">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" rows="4" placeholder="Why would you like to volunteer?" required></textarea>
            <button type="submit" class="btn-gradient">Sign Up</button>
        </form>
    </section>

    <footer>
        <h2 class="section-title">Stay Updated</h2>
        <div class="social-icons">
            <a href="https://instagram.com/YOUR_HANDLE" target="_blank"><i class="fab fa-instagram"></i></a>
            <a href="https://twitter.com/YOUR_HANDLE" target="_blank"><i class="fab fa-x-twitter"></i></a>
            <a href="https://facebook.com/YOUR_HANDLE" target="_blank"><i class="fab fa-facebook-f"></i></a>
        </div>
        <a href="https://twitter.com/YOUR_HANDLE" class="social-handle" target="_blank">@YourTwitterHandle</a>
        <div class="footer-info">
            <p>© 2025 Frontline | Built with dedication for humanitarian aid.</p>
            <p style="font-style: italic; margin-top: 10px;">"Small things with great love."</p>
        </div>
    </footer>

</body>
</html>

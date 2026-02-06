<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Taher Husain | Real Estate Advisor</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;600;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        :root {
            --gold: #C5A059;
            --navy: #0A192F;
            --slate: #4A5568;
            --off-white: #F8F9FA;
            --white: #FFFFFF;
        }

        * { box-sizing: border-box; }
        body { 
            font-family: 'Montserrat', sans-serif; 
            background-color: #E2E8F0; 
            margin: 0; 
            padding: 0; 
            color: var(--navy); 
        }

        .container {
            max-width: 800px;
            margin: 20px auto;
            background: var(--white);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }

        /* --- Header Section --- */
        .header {
            background: linear-gradient(135deg, var(--navy) 0%, #162C4E 100%);
            padding: 60px 20px;
            text-align: center;
            color: var(--white);
            position: relative;
        }

        .profile-img {
            width: 160px;
            height: 160px;
            border-radius: 50%;
            border: 4px solid var(--gold);
            object-fit: cover;
            margin-bottom: 20px;
            box-shadow: 0 10px 20px rgba(0,0,0,0.3);
            /* Updated image path to your GitHub name */
            background-image: url('Taher.jpg');
            background-size: cover;
        }

        .header h1 {
            font-family: 'Playfair Display', serif;
            font-size: 2.8rem;
            margin: 0;
            letter-spacing: 1px;
            color: var(--gold);
        }

        .header p {
            font-size: 1.1rem;
            font-weight: 300;
            margin: 10px 0;
            opacity: 0.9;
        }

        .badge-bar {
            margin-top: 20px;
            display: flex;
            justify-content: center;
            gap: 10px;
            flex-wrap: wrap;
        }

        .badge {
            background: rgba(197, 160, 89, 0.2);
            border: 1px solid var(--gold);
            padding: 6px 15px;
            border-radius: 30px;
            font-size: 0.8rem;
            font-weight: 600;
            color: var(--gold);
        }

        /* --- Content Sections --- */
        .section { padding: 40px 30px; }
        .section-title {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            border-bottom: 2px solid var(--gold);
            display: inline-block;
            margin-bottom: 25px;
            color: var(--navy);
        }

        .intro-text {
            font-size: 1.05rem;
            line-height: 1.8;
            color: var(--slate);
        }

        /* --- Skills Grid --- */
        .grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        .card {
            background: var(--off-white);
            padding: 20px;
            border-radius: 12px;
            border-top: 4px solid var(--gold);
        }

        .card h3 { font-size: 1rem; margin-top: 0; color: var(--navy); text-transform: uppercase; }
        .card ul { padding-left: 18px; margin-bottom: 0; color: var(--slate); font-size: 0.9rem; }
        .card li { margin-bottom: 8px; }

        /* --- Experience Timeline --- */
        .timeline-item {
            margin-bottom: 30px;
            padding-left: 20px;
            border-left: 2px solid #E2E8F0;
            position: relative;
        }

        .timeline-item::before {
            content: '';
            position: absolute;
            left: -7px;
            top: 0;
            width: 12px;
            height: 12px;
            background: var(--gold);
            border-radius: 50%;
        }

        .role { font-weight: 700; font-size: 1.1rem; margin: 0; }
        .company { color: var(--gold); font-weight: 600; font-size: 0.95rem; margin: 4px 0; }
        .desc { font-size: 0.9rem; color: var(--slate); line-height: 1.5; }

        /* --- Footer & Contact --- */
        .footer {
            background: var(--navy);
            color: var(--white);
            padding: 50px 30px;
            text-align: center;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .contact-link {
            text-decoration: none;
            color: var(--white);
            background: rgba(255,255,255,0.05);
            padding: 15px;
            border-radius: 10px;
            border: 1px solid rgba(197,160,89,0.3);
            transition: 0.3s;
            display: block;
        }

        .contact-link:hover {
            background: var(--gold);
            color: var(--navy);
        }

        /* --- Mobile Responsiveness --- */
        @media (max-width: 600px) {
            .grid { grid-template-columns: 1fr; }
            .header h1 { font-size: 2.2rem; }
            .section { padding: 30px 20px; }
        }
    </style>
</head>
<body>

<div class="container">
    <header class="header">
        <div style="display: flex; justify-content: center;">
            <div class="profile-img"></div>
        </div>
        <h1>Taher Husain</h1>
        <p>Premium Real Estate Advisor | Visionary Entrepreneur</p>
        <div class="badge-bar">
            <span class="badge">🇦🇪 Investor Visa</span>
            <span class="badge">📍 Dubai Resident</span>
            <span class="badge">🚗 LMV Licensed</span>
        </div>
    </header>

    <section class="section">
        <h2 class="section-title">Elevating Your Dubai Experience</h2>
        <p class="intro-text">
            Transitioning from 7+ years of successful business ownership into the Dubai real estate market, I bring a unique <strong>entrepreneurial edge</strong> to property advisory. My philosophy is simple: I don't just sell property; I build partnerships based on <strong>transparency, strategic insight, and high-level negotiation</strong>. Whether you are looking for a luxury home or a high-yield investment, I apply the same rigor that made my import/export ventures successful to ensure your assets are protected and your goals are met.
        </p>
    </section>

    <section class="section" style="background-color: #fcfcfc;">
        <h2 class="section-title">Core Expertise</h2>
        <div class="grid">
            <div class="card">
                <h3>🏠 Real Estate Strategy</h3>
                <ul>
                    <li>Dynamic Market Analysis</li>
                    <li>Property Advisory & Valuation</li>
                    <li>Bespoke Viewing Experiences</li>
                    <li>Seamless Documentation Management</li>
                </ul>
            </div>
            <div class="card">
                <h3>🤝 Business Acumen</h3>
                <ul>
                    <li>Strategic Win-Win Negotiation</li>
                    <li>Global Client Relations</li>
                    <li>Complex Deal Structuring</li>
                    <li>Investment Risk Assessment</li>
                </ul>
            </div>
        </div>
    </section>

    <section class="section">
        <h2 class="section-title">Professional Journey</h2>
        
        <div class="timeline-item">
            <p class="role">Founder & Managing Director</p>
            <p class="company">Al Mubarak Al Tijarah FZ LLC | 2023 – Present</p>
            <p class="desc">Spearheading a thriving international trade enterprise. This experience serves as my foundation for managing high-value transactions and understanding the speed of Dubai's economy.</p>
        </div>

        <div class="timeline-item">
            <p class="role">Business Partner</p>
            <p class="company">Al Marzaan General Trading | 2022 – 2023</p>
            <p class="desc">Managed high-stakes B2B negotiations and long-term business partnerships across the UAE.</p>
        </div>

        <div class="timeline-item">
            <p class="role">Operational Leadership</p>
            <p class="company">Previous Roles (2016 – 2022)</p>
            <p class="desc">Leadership roles at Cravers Kitchen and Anjuman E Najmi, focusing on organizational excellence and client satisfaction.</p>
        </div>
    </section>

    <section class="section" style="background: #F8F9FA; text-align: center;">
        <p style="font-style: italic; color: var(--slate);">
            "Beyond business, my heart lies in community service. This dedication to helping others ensures that my real estate approach is always client-first, ethical, and empathetic."
        </p>
        <div style="margin-top: 20px; font-size: 0.85rem; color: var(--slate);">
            <strong>Languages:</strong> English, Hindi, Urdu | <strong>Nationality:</strong> Indian
        </div>
    </section>

    <footer class="footer">
        <h2 style="font-family: 'Playfair Display', serif; color: var(--gold); margin-bottom: 10px;">Let’s Connect</h2>
        <p>Ready to start your property journey in Dubai?</p>
        
        <div class="contact-grid">
            <a href="https://wa.me/971521790412" class="contact-link">💬 WhatsApp</a>
            <a href="tel:+971581130453" class="contact-link">📞 Call Me</a>
            <a href="mailto:tbetwala29@gmail.com" class="contact-link">✉️ Email Me</a>
        </div>

        <p style="font-size: 0.7rem; margin-top: 40px; opacity: 0.6;">
            Last Updated 2026 | Professional Digital Profile
        </p>
    </footer>
</div>

</body>
</html>

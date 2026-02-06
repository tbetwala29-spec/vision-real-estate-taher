<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Taher - Real Estate Sales Executive</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Montserrat:wght@400;500;700&family=Playfair+Display:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #3a506b;
            --secondary: #5bc0be;
            --accent: #6fffe9;
            --light: #f8f9fa;
            --dark: #1c2541;
            --highlight: #ff9f1c;
            --bg-gradient: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
            --card-shadow: 0 8px 25px rgba(0, 0, 0, 0.08);
            --transition: all 0.3s ease;
            --gold: #d4af37;
            --sand: #f5e8c8;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: #444;
            background-color: #fefefe;
            overflow-x: hidden;
            background-image: radial-gradient(#e9ecef 1px, transparent 1px);
            background-size: 20px 20px;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Header Styles */
        header {
            background: white;
            color: var(--dark);
            padding: 40px 0;
            border-bottom: 1px solid rgba(0, 0, 0, 0.05);
            margin-bottom: 40px;
            position: relative;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.03);
            border-radius: 0 0 15px 15px;
        }

        .header-content {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: space-between;
        }

        .profile-section {
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            gap: 40px;
            width: 100%;
        }

        .profile-img-container {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            border: 6px solid white;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            transition: var(--transition);
            position: relative;
            z-index: 1;
        }

        .profile-img-container:hover {
            transform: scale(1.03);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.15);
        }

        .profile-img-container::before {
            content: '';
            position: absolute;
            top: -6px;
            left: -6px;
            right: -6px;
            bottom: -6px;
            background: linear-gradient(45deg, var(--secondary), var(--accent));
            border-radius: 50%;
            z-index: -1;
        }

        .profile-img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .profile-text {
            flex: 1;
            min-width: 300px;
        }

        .name {
            font-family: 'Playfair Display', serif;
            font-size: 2.8rem;
            font-weight: 700;
            margin-bottom: 5px;
            color: var(--dark);
            background: linear-gradient(90deg, var(--dark), var(--primary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .title {
            font-size: 1.4rem;
            font-weight: 500;
            margin-bottom: 15px;
            color: var(--primary);
            position: relative;
            display: inline-block;
        }

        .title::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 50px;
            height: 3px;
            background-color: var(--highlight);
        }

        .contact-info {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 20px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 10px;
            font-size: 0.95rem;
            background: white;
            padding: 10px 18px;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
            transition: var(--transition);
            border: 1px solid #eee;
        }

        .contact-item:hover {
            background: #f8f9fa;
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.08);
        }

        .contact-item i {
            color: var(--secondary);
        }

        .visa-badge {
            display: inline-block;
            background-color: var(--sand);
            color: var(--dark);
            padding: 8px 20px;
            border-radius: 8px;
            font-weight: 600;
            font-size: 0.9rem;
            margin-top: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.05);
            border-left: 4px solid var(--gold);
        }

        /* Call to Action Buttons */
        .cta-buttons {
            display: flex;
            gap: 15px;
            margin-top: 25px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            padding: 12px 25px;
            border-radius: 8px;
            font-weight: 600;
            font-size: 0.95rem;
            text-decoration: none;
            transition: var(--transition);
            border: none;
            cursor: pointer;
        }

        .btn-call {
            background: linear-gradient(to right, #25D366, #128C7E);
            color: white;
            box-shadow: 0 4px 15px rgba(37, 211, 102, 0.2);
        }

        .btn-call:hover {
            background: linear-gradient(to right, #128C7E, #25D366);
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(37, 211, 102, 0.3);
        }

        .btn-whatsapp {
            background: linear-gradient(to right, #34B7F1, #25D366);
            color: white;
            box-shadow: 0 4px 15px rgba(37, 211, 102, 0.2);
        }

        .btn-whatsapp:hover {
            background: linear-gradient(to right, #25D366, #34B7F1);
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(37, 211, 102, 0.3);
        }

        .btn-email {
            background: linear-gradient(to right, var(--primary), var(--dark));
            color: white;
            box-shadow: 0 4px 15px rgba(58, 80, 107, 0.2);
        }

        .btn-email:hover {
            background: linear-gradient(to right, var(--dark), var(--primary));
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(58, 80, 107, 0.3);
        }

        /* Section Styles */
        section {
            background: white;
            border-radius: 15px;
            padding: 35px;
            margin-bottom: 30px;
            box-shadow: var(--card-shadow);
            transition: var(--transition);
            border: 1px solid rgba(0, 0, 0, 0.03);
        }

        section:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.1);
        }

        .section-title {
            font-family: 'Playfair Display', serif;
            font-size: 1.9rem;
            color: var(--primary);
            margin-bottom: 25px;
            padding-bottom: 12px;
            border-bottom: 2px solid var(--sand);
            display: inline-block;
            position: relative;
        }

        .section-title i {
            margin-right: 10px;
            color: var(--secondary);
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -2px;
            left: 0;
            width: 70px;
            height: 2px;
            background-color: var(--highlight);
        }

        /* Professional Summary */
        .summary-text {
            font-size: 1.1rem;
            line-height: 1.8;
            color: #555;
        }

        .highlight {
            color: var(--secondary);
            font-weight: 600;
            background-color: rgba(91, 192, 190, 0.1);
            padding: 2px 6px;
            border-radius: 4px;
        }

        /* Core Competencies */
        .competencies-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }

        .competency-item {
            background: white;
            padding: 22px;
            border-radius: 10px;
            border-left: 5px solid var(--secondary);
            transition: var(--transition);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.03);
            border: 1px solid #f0f0f0;
        }

        .competency-item:hover {
            border-left-color: var(--highlight);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.08);
        }

        .competency-item h3 {
            font-size: 1.2rem;
            color: var(--primary);
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .competency-item h3 i {
            color: var(--secondary);
            width: 24px;
            text-align: center;
        }

        /* Experience */
        .experience-item {
            margin-bottom: 30px;
            padding-bottom: 25px;
            border-bottom: 1px solid #eee;
            position: relative;
        }

        .experience-item:last-child {
            border-bottom: none;
            padding-bottom: 0;
        }

        .experience-item::before {
            content: '';
            position: absolute;
            left: -15px;
            top: 5px;
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background-color: var(--accent);
        }

        .exp-header {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            margin-bottom: 10px;
        }

        .company {
            font-size: 1.3rem;
            font-weight: 600;
            color: var(--primary);
        }

        .period {
            background-color: var(--sand);
            color: var(--dark);
            padding: 6px 18px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 500;
        }

        .role {
            font-size: 1.1rem;
            color: var(--secondary);
            margin-bottom: 15px;
            font-style: italic;
            font-weight: 500;
        }

        .responsibilities {
            list-style-type: none;
        }

        .responsibilities li {
            margin-bottom: 12px;
            padding-left: 28px;
            position: relative;
        }

        .responsibilities li:before {
            content: "▸";
            color: var(--accent);
            font-size: 1.3rem;
            position: absolute;
            left: 0;
            font-weight: bold;
        }

        /* Community & Education */
        .community-section, .education-section {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
        }

        .community-text, .education-item {
            flex: 1;
            min-width: 300px;
        }

        .education-item {
            background: white;
            padding: 22px;
            border-radius: 10px;
            border: 1px solid #f0f0f0;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.03);
            transition: var(--transition);
        }

        .education-item:hover {
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.08);
        }

        /* Personal Details */
        .personal-details {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
        }

        .detail-item {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 18px;
            background: white;
            border-radius: 10px;
            transition: var(--transition);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.03);
            border: 1px solid #f0f0f0;
        }

        .detail-item:hover {
            transform: translateX(5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.08);
            border-left: 4px solid var(--secondary);
        }

        .detail-item i {
            font-size: 1.6rem;
            color: var(--secondary);
            width: 40px;
            text-align: center;
        }

        .detail-label {
            font-weight: 600;
            color: var(--primary);
            margin-bottom: 5px;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 40px 0;
            margin-top: 40px;
            background: linear-gradient(to right, var(--primary), var(--dark));
            color: white;
            border-radius: 15px 15px 0 0;
            position: relative;
            overflow: hidden;
        }

        footer::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(to right, var(--accent), var(--highlight));
        }

        .footer-text {
            font-size: 0.95rem;
            opacity: 0.9;
            margin-top: 10px;
        }

        /* Responsive Design */
        @media (max-width: 992px) {
            .profile-section {
                flex-direction: column;
                text-align: center;
            }
            
            .profile-text {
                text-align: center;
            }
            
            .title::after {
                left: 50%;
                transform: translateX(-50%);
            }
            
            .contact-info {
                justify-content: center;
            }
            
            .cta-buttons {
                justify-content: center;
            }
        }

        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
            }

            .name {
                font-size: 2.2rem;
            }

            .title {
                font-size: 1.2rem;
            }

            .section-title {
                font-size: 1.6rem;
            }

            .exp-header {
                flex-direction: column;
                gap: 10px;
            }

            .period {
                align-self: flex-start;
            }
            
            .profile-img-container {
                width: 170px;
                height: 170px;
            }
            
            section {
                padding: 25px;
            }
        }

        @media (max-width: 480px) {
            .container {
                width: 95%;
                padding: 15px;
            }

            .competencies-grid {
                grid-template-columns: 1fr;
            }

            .profile-img-container {
                width: 150px;
                height: 150px;
            }
            
            .btn {
                width: 100%;
                justify-content: center;
            }
            
            .cta-buttons {
                flex-direction: column;
            }
        }

        /* Animation for page load */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .fade-in {
            animation: fadeIn 0.8s ease forwards;
        }
        
        /* Floating elements */
        .floating-element {
            position: absolute;
            background: rgba(255, 255, 255, 0.7);
            border-radius: 50%;
            z-index: -1;
        }
        
        .floating-1 {
            width: 100px;
            height: 100px;
            top: 10%;
            right: 5%;
            background: radial-gradient(circle, var(--accent) 0%, transparent 70%);
            opacity: 0.2;
        }
        
        .floating-2 {
            width: 150px;
            height: 150px;
            bottom: 10%;
            left: 5%;
            background: radial-gradient(circle, var(--secondary) 0%, transparent 70%);
            opacity: 0.1;
        }
    </style>
</head>
<body>
    <!-- Floating Background Elements -->
    <div class="floating-element floating-1"></div>
    <div class="floating-element floating-2"></div>
    
    <div class="container">
        <!-- Header with Profile -->
        <header class="fade-in">
            <div class="header-content">
                <div class="profile-section">
                    <div class="profile-img-container">
                        <!-- Using the provided image from GitHub -->
                        <img src="Taher.jpg" alt="Taher - Real Estate Professional" class="profile-img" onerror="this.src='https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=774&q=80'">
                    </div>
                    <div class="profile-text">
                        <h1 class="name">Taher Betwala</h1>
                        <div class="title">Real Estate Sales Executive Candidate</div>
                        <div class="visa-badge">Visa Status: Investor</div>
                        
                        <div class="contact-info">
                            <div class="contact-item">
                                <i class="fas fa-map-marker-alt"></i>
                                <span>Dubai, UAE</span>
                            </div>
                            <div class="contact-item">
                                <i class="fas fa-phone"></i>
                                <span>+971 58 113 0453</span>
                            </div>
                            <div class="contact-item">
                                <i class="fas fa-comment-alt"></i>
                                <span>+971 52 179 0412</span>
                            </div>
                            <div class="contact-item">
                                <i class="fas fa-envelope"></i>
                                <span>tbetwala29@gmail.com</span>
                            </div>
                        </div>
                        
                        <!-- Call to Action Buttons -->
                        <div class="cta-buttons">
                            <a href="tel:+971581130453" class="btn btn-call">
                                <i class="fas fa-phone-alt"></i> Call Now
                            </a>
                            <a href="https://wa.me/971581130453?text=Hi%20Taher,%20I'm%20interested%20in%20discussing%20real%20estate%20opportunities" target="_blank" class="btn btn-whatsapp">
                                <i class="fab fa-whatsapp"></i> WhatsApp
                            </a>
                            <a href="mailto:tbetwala29@gmail.com" class="btn btn-email">
                                <i class="fas fa-envelope"></i> Email
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </header>

        <!-- Professional Summary -->
        <section class="fade-in">
            <h2 class="section-title"><i class="fas fa-user-tie"></i> PROFESSIONAL SUMMARY</h2>
            <div class="summary-text">
                A dynamic and results-driven Entrepreneur with over <span class="highlight">8 years of experience in the Dubai market</span> across general trading, operations, and administration. Proven track record in high-stakes negotiation, client relationship management, and complex supply chain logistics. As an active <span class="highlight">Social Worker</span> within the local community, I possess a deep-rooted network and exceptional interpersonal skills. Transitioning into Real Estate with a commitment to leveraging my local market expertise and <span class="highlight">"investor mindset"</span> to drive sales and deliver premium service to property investors and end-users.
            </div>
        </section>

        <!-- Core Competencies -->
        <section class="fade-in">
            <h2 class="section-title"><i class="fas fa-star"></i> CORE COMPETENCIES</h2>
            <div class="competencies-grid">
                <div class="competency-item">
                    <h3><i class="fas fa-handshake"></i> Sales & Negotiation</h3>
                    <p>Highly proficient at closing deals and managing pricing discussions with a collaborative approach.</p>
                </div>
                <div class="competency-item">
                    <h3><i class="fas fa-users"></i> Relationship Management</h3>
                    <p>Built a loyal client base through trust and transparency with long-term relationship focus.</p>
                </div>
                <div class="competency-item">
                    <h3><i class="fas fa-map-marked-alt"></i> Local Market Knowledge</h3>
                    <p>Deep understanding of Dubai's business landscape and residential areas with on-ground experience.</p>
                </div>
                <div class="competency-item">
                    <h3><i class="fas fa-cogs"></i> Operational Excellence</h3>
                    <p>Full-cycle business management, from sourcing to final delivery with systematic approach.</p>
                </div>
                <div class="competency-item">
                    <h3><i class="fas fa-hands-helping"></i> Community Leadership</h3>
                    <p>Respected social worker with strong networking capabilities and community trust.</p>
                </div>
                <div class="competency-item">
                    <h3><i class="fas fa-language"></i> Languages</h3>
                    <p>Fluent in English, Hindi, and Urdu for effective multicultural communication.</p>
                </div>
            </div>
        </section>

        <!-- Professional Experience -->
        <section class="fade-in">
            <h2 class="section-title"><i class="fas fa-briefcase"></i> PROFESSIONAL EXPERIENCE</h2>
            
            <div class="experience-item">
                <div class="exp-header">
                    <div class="company">Al Mubarak Al Tijarah FZ LLC, Dubai</div>
                    <div class="period">2023 – Present</div>
                </div>
                <div class="role">Founder / Managing Director</div>
                <p><em>Specializing in the import, export, and wholesale distribution of fresh produce.</em></p>
                <ul class="responsibilities">
                    <li>Independently managed the entire business lifecycle, including global sourcing and local supply chain.</li>
                    <li>Established a robust B2C and B2B network, supplying premium fresh fruits and vegetables to families and catering companies across the UAE.</li>
                    <li>Mastered the art of "Personal Selling," building a business from the ground up through direct client engagement and word-of-mouth referrals.</li>
                </ul>
            </div>
            
            <div class="experience-item">
                <div class="exp-header">
                    <div class="company">Al Marzaan General Trading, Dubai</div>
                    <div class="period">2022 – 2023</div>
                </div>
                <div class="role">Business Partner</div>
                <ul class="responsibilities">
                    <li>Developed strategic sales plans that led to significant growth in client acquisition.</li>
                    <li>Managed supplier relationships and negotiated high-volume contracts.</li>
                    <li>Handled day-to-day business reporting and operational oversight to ensure 100% customer satisfaction.</li>
                </ul>
            </div>
            
            <div class="experience-item">
                <div class="exp-header">
                    <div class="company">Cravers Kitchen, Dubai</div>
                    <div class="period">2021 – 2022</div>
                </div>
                <div class="role">Manager</div>
                <ul class="responsibilities">
                    <li>Directed daily operations and staff coordination in a fast-paced environment.</li>
                    <li>Boosted customer retention rates by implementing a "client-first" communication strategy.</li>
                </ul>
            </div>
            
            <div class="experience-item">
                <div class="exp-header">
                    <div class="company">Anjuman E Najmi, Dubai</div>
                    <div class="period">2016 – 2021</div>
                </div>
                <div class="role">Administrator</div>
                <ul class="responsibilities">
                    <li>Managed high-level administrative functions and stakeholder communications.</li>
                    <li>Maintained sensitive databases and coordinated between internal departments and external community members.</li>
                </ul>
            </div>
        </section>

        <!-- Community & Volunteering -->
        <section class="fade-in">
            <h2 class="section-title"><i class="fas fa-hands-helping"></i> COMMUNITY & VOLUNTEERING</h2>
            <div class="community-section">
                <div class="community-text">
                    <h3>Active Community Social Worker</h3>
                    <p>Dedicated to supporting community initiatives and fostering social welfare. This role has allowed me to build a vast network of trust-based relationships across Dubai, providing a unique advantage in identifying potential real estate leads and understanding family housing needs.</p>
                </div>
            </div>
        </section>

        <!-- Education & Licenses -->
        <section class="fade-in">
            <h2 class="section-title"><i class="fas fa-graduation-cap"></i> EDUCATION & LICENSES</h2>
            <div class="education-section">
                <div class="education-item">
                    <h3><i class="fas fa-certificate"></i> Higher Secondary Education</h3>
                    <p>Completed</p>
                </div>
                <div class="education-item">
                    <h3><i class="fas fa-car"></i> UAE Driving License</h3>
                    <p>Valid LMV License (essential for property viewings)</p>
                </div>
            </div>
        </section>

        <!-- Personal Details -->
        <section class="fade-in">
            <h2 class="section-title"><i class="fas fa-user-circle"></i> PERSONAL DETAILS</h2>
            <div class="personal-details">
                <div class="detail-item">
                    <i class="fas fa-globe"></i>
                    <div>
                        <div class="detail-label">Nationality</div>
                        <div>Indian</div>
                    </div>
                </div>
                <div class="detail-item">
                    <i class="fas fa-heart"></i>
                    <div>
                        <div class="detail-label">Marital Status</div>
                        <div>Married</div>
                    </div>
                </div>
                <div class="detail-item">
                    <i class="fas fa-birthday-cake"></i>
                    <div>
                        <div class="detail-label">Date of Birth</div>
                        <div>10 July 1988</div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer class="fade-in">
            <p>© <span id="currentYear"></span> Taher Betwala - Real Estate Sales Executive</p>
            <p class="footer-text">Dubai, UAE | Ready to contribute to your real estate success</p>
            <div class="cta-buttons" style="margin-top: 25px; justify-content: center;">
                <a href="tel:+971581130453" class="btn btn-call">
                    <i class="fas fa-phone-alt"></i> Call +971 58 113 0453
                </a>
                <a href="https://wa.me/971581130453?text=Hi%20Taher,%20I'm%20interested%20in%20discussing%20real%20estate%20opportunities" target="_blank" class="btn btn-whatsapp">
                    <i class="fab fa-whatsapp"></i> WhatsApp Me
                </a>
            </div>
        </footer>
    </div>

    <script>
        // Set current year in footer
        document.getElementById('currentYear').textContent = new Date().getFullYear();
        
        // Add fade-in animation to sections on scroll
        document.addEventListener('DOMContentLoaded', function() {
            const fadeElements = document.querySelectorAll('.fade-in');
            
            const fadeInOnScroll = function() {
                fadeElements.forEach(element => {
                    const elementTop = element.getBoundingClientRect().top;
                    const elementVisible = 150;
                    
                    if (elementTop < window.innerHeight - elementVisible) {
                        element.style.opacity = "1";
                        element.style.transform = "translateY(0)";
                    }
                });
            };
            
            // Set initial state
            fadeElements.forEach(element => {
                element.style.opacity = "0";
                element.style.transform = "translateY(20px)";
                element.style.transition = "opacity 0.8s ease, transform 0.8s ease";
            });
            
            // Check on scroll and load
            window.addEventListener('scroll', fadeInOnScroll);
            fadeInOnScroll(); // Run on initial load
            
            // Add smooth scrolling for anchor links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function(e) {
                    e.preventDefault();
                    const targetId = this.getAttribute('href');
                    if(targetId === '#') return;
                    const targetElement = document.querySelector(targetId);
                    if(targetElement) {
                        window.scrollTo({
                            top: targetElement.offsetTop - 80,
                            behavior: 'smooth'
                        });
                    }
                });
            });
        });
    </script>
</body>
</html>

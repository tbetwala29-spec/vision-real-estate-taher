<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Taher - Real Estate Sales Executive</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Montserrat:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #2c3e50;
            --secondary: #e74c3c;
            --accent: #3498db;
            --light: #ecf0f1;
            --dark: #2c3e50;
            --highlight: #f39c12;
            --bg-gradient: linear-gradient(135deg, #1a2980 0%, #26d0ce 100%);
            --card-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f9f9f9;
            overflow-x: hidden;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Header Styles */
        header {
            background: var(--bg-gradient);
            color: white;
            padding: 30px 0;
            border-bottom-left-radius: 20px;
            border-bottom-right-radius: 20px;
            box-shadow: var(--card-shadow);
            margin-bottom: 40px;
            position: relative;
            overflow: hidden;
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
            gap: 30px;
        }

        .profile-img-container {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            border: 5px solid rgba(255, 255, 255, 0.3);
            overflow: hidden;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.2);
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
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
            font-family: 'Montserrat', sans-serif;
            font-size: 2.5rem;
            font-weight: 700;
            margin-bottom: 5px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
        }

        .title {
            font-size: 1.5rem;
            font-weight: 500;
            margin-bottom: 15px;
            color: rgba(255, 255, 255, 0.9);
        }

        .contact-info {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 15px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 0.95rem;
            background: rgba(255, 255, 255, 0.15);
            padding: 8px 15px;
            border-radius: 30px;
            backdrop-filter: blur(5px);
            transition: var(--transition);
        }

        .contact-item:hover {
            background: rgba(255, 255, 255, 0.25);
            transform: translateY(-3px);
        }

        .contact-item i {
            color: var(--highlight);
        }

        .visa-badge {
            display: inline-block;
            background-color: var(--highlight);
            color: var(--dark);
            padding: 5px 15px;
            border-radius: 20px;
            font-weight: 600;
            font-size: 0.9rem;
            margin-top: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        /* Section Styles */
        section {
            background: white;
            border-radius: 15px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: var(--card-shadow);
            transition: var(--transition);
        }

        section:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.1);
        }

        .section-title {
            font-family: 'Montserrat', sans-serif;
            font-size: 1.8rem;
            color: var(--primary);
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 3px solid var(--accent);
            display: inline-block;
        }

        .section-title i {
            margin-right: 10px;
            color: var(--secondary);
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
        }

        /* Core Competencies */
        .competencies-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }

        .competency-item {
            background: linear-gradient(to right, #f8f9fa, #e9ecef);
            padding: 20px;
            border-radius: 10px;
            border-left: 5px solid var(--accent);
            transition: var(--transition);
        }

        .competency-item:hover {
            background: linear-gradient(to right, #e9ecef, #dee2e6);
            border-left-color: var(--secondary);
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
        }

        /* Experience */
        .experience-item {
            margin-bottom: 30px;
            padding-bottom: 20px;
            border-bottom: 1px dashed #ddd;
        }

        .experience-item:last-child {
            border-bottom: none;
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
            background-color: var(--primary);
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
        }

        .role {
            font-size: 1.1rem;
            color: var(--secondary);
            margin-bottom: 15px;
            font-style: italic;
        }

        .responsibilities {
            list-style-type: none;
        }

        .responsibilities li {
            margin-bottom: 10px;
            padding-left: 25px;
            position: relative;
        }

        .responsibilities li:before {
            content: "▸";
            color: var(--accent);
            font-size: 1.2rem;
            position: absolute;
            left: 0;
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
            background: linear-gradient(to bottom right, #f8f9fa, #e9ecef);
            padding: 20px;
            border-radius: 10px;
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
            padding: 15px;
            background: #f8f9fa;
            border-radius: 10px;
            transition: var(--transition);
        }

        .detail-item:hover {
            background: #e9ecef;
            transform: translateX(5px);
        }

        .detail-item i {
            font-size: 1.5rem;
            color: var(--accent);
            width: 40px;
            text-align: center;
        }

        .detail-label {
            font-weight: 600;
            color: var(--primary);
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 30px 0;
            margin-top: 40px;
            background: var(--primary);
            color: white;
            border-radius: 15px 15px 0 0;
        }

        .footer-text {
            font-size: 0.9rem;
            opacity: 0.8;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }

            .profile-section {
                flex-direction: column;
                text-align: center;
            }

            .contact-info {
                justify-content: center;
            }

            .name {
                font-size: 2rem;
            }

            .title {
                font-size: 1.2rem;
            }

            .section-title {
                font-size: 1.5rem;
            }

            .exp-header {
                flex-direction: column;
                gap: 10px;
            }

            .period {
                align-self: flex-start;
            }
        }

        @media (max-width: 480px) {
            .container {
                width: 95%;
                padding: 10px;
            }

            section {
                padding: 20px;
            }

            .competencies-grid {
                grid-template-columns: 1fr;
            }

            .profile-img-container {
                width: 150px;
                height: 150px;
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
    </style>
</head>
<body>
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
                    <p>Expert at closing deals and managing pricing discussions.</p>
                </div>
                <div class="competency-item">
                    <h3><i class="fas fa-users"></i> Relationship Management</h3>
                    <p>Built a loyal client base through trust and transparency.</p>
                </div>
                <div class="competency-item">
                    <h3><i class="fas fa-map-marked-alt"></i> Local Market Knowledge</h3>
                    <p>Deep understanding of Dubai's business landscape and residential areas.</p>
                </div>
                <div class="competency-item">
                    <h3><i class="fas fa-cogs"></i> Operational Excellence</h3>
                    <p>Full-cycle business management, from sourcing to final delivery.</p>
                </div>
                <div class="competency-item">
                    <h3><i class="fas fa-hands-helping"></i> Community Leadership</h3>
                    <p>Respected social worker with strong networking capabilities.</p>
                </div>
                <div class="competency-item">
                    <h3><i class="fas fa-language"></i> Languages</h3>
                    <p>Fluent in English, Hindi, and Urdu.</p>
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
        });
    </script>
</body>
</html>

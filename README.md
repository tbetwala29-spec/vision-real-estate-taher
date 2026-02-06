<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
  body { font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; background-color: #f4f4f7; color: #333; margin: 0; padding: 10px; }
  .profile-card { max-width: 650px; margin: 20px auto; background: white; border-radius: 16px; overflow: hidden; box-shadow: 0 10px 30px rgba(0,0,0,0.1); border: 1px solid #e1e1e1; }
  
  /* Header Section */
  .header { background: #0a192f; padding: 40px 20px; text-align: center; color: #fff; }
  .profile-img { width: 150px; height: 150px; border-radius: 50%; border: 3px solid #c5a059; object-fit: cover; margin-bottom: 15px; box-shadow: 0 4px 10px rgba(0,0,0,0.3); }
  .name { font-size: 2.2em; font-weight: 700; letter-spacing: 1px; color: #c5a059; margin: 10px 0 5px 0; text-transform: uppercase; }
  .tagline { font-size: 1.1em; color: #e0e0e0; font-weight: 300; margin-bottom: 20px; }
  
  /* Badges */
  .badge-container { display: flex; flex-wrap: wrap; justify-content: center; gap: 8px; }
  .badge { background: rgba(197, 160, 89, 0.15); color: #c5a059; padding: 6px 14px; border-radius: 50px; font-size: 0.85em; font-weight: 600; border: 1px solid #c5a059; }

  /* Body Content */
  .content { padding: 30px 25px; }
  h2 { color: #0a192f; border-bottom: 2px solid #c5a059; display: inline-block; padding-bottom: 5px; font-size: 1.3em; margin-bottom: 20px; text-transform: uppercase; }
  p { line-height: 1.6; color: #444; }

  /* Grid for Skills - Responsive */
  .skills-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin: 20px 0; }
  @media (max-width: 500px) { .skills-grid { grid-template-columns: 1fr; } }
  
  .skill-box { background: #f9fafb; padding: 15px; border-radius: 12px; border-left: 4px solid #0a192f; }
  .skill-box h4 { margin-top: 0; color: #c5a059; font-size: 0.95em; }
  .skill-list { list-style: none; padding: 0; font-size: 0.9em; margin: 0; }
  .skill-list li { margin-bottom: 8px; position: relative; padding-left: 15px; }
  .skill-list li::before { content: "•"; color: #c5a059; position: absolute; left: 0; font-weight: bold; }

  /* Experience Section */
  .exp-item { margin-bottom: 25px; padding-left: 15px; border-left: 1px solid #ddd; }
  .exp-title { font-weight: 700; color: #0a192f; font-size: 1.1em; margin: 0; }
  .exp-company { color: #c5a059; font-weight: 600; font-size: 0.9em; margin: 2px 0; }
  .exp-desc { font-size: 0.95em; color: #666; }

  /* Contact Footer */
  .footer { background: #f0f2f5; padding: 30px 20px; text-align: center; }
  .cta-btn { background: #0a192f; color: #c5a059; padding: 12px 25px; border-radius: 8px; text-decoration: none; display: inline-block; font-weight: bold; margin-bottom: 20px; border: 1px solid #c5a059; }
  .contact-info { font-size: 0.95em; color: #333; line-height: 2; }
  .contact-info strong { color: #0a192f; }
</style>
</head>
<body>

<div class="profile-card">
  <div class="header">
    <img src="Taher.jpg" alt="Taher Husain" class="profile-img">
    <div class="name">Taher Husain</div>
    <div class="tagline">Premium Property Advisor | Entrepreneur</div>
    <div class="badge-container">
      <span class="badge">📍 Dubai, UAE</span>
      <span class="badge">🇦🇪 Investor Visa</span>
      <span class="badge">🚗 LMV Licensed</span>
    </div>
  </div>

  <div class="content">
    <h2>Professional Profile</h2>
    <p>
      With over <strong>7 years of entrepreneurial success</strong> in Dubai, I bring a refined business acumen to the real estate sector. Having founded and managed international trading operations, I specialize in the art of the deal—combining <strong>strategic negotiation</strong> with a deep-rooted commitment to client trust.
    </p>

    <div class="skills-grid">
      <div class="skill-box">
        <h4>COMMERCIAL EXPERTISE</h4>
        <ul class="skill-list">
          <li>Strategic Negotiation</li>
          <li>Market Analysis</li>
          <li>Investment Sourcing</li>
          <li>Complex Transactions</li>
        </ul>
      </div>
      <div class="skill-box">
        <h4>CLIENT ADVOCACY</h4>
        <ul class="skill-list">
          <li>Relationship Management</li>
          <li>Clear Communication</li>
          <li>Problem Solving</li>
          <li>Integrity-Driven Results</li>
        </ul>
      </div>
    </div>

    <h2>Experience</h2>
    
    <div class="exp-item">
      <p class="exp-title">Founder & Managing Director</p>
      <p class="exp-company">Al Mubarak Al Tijarah FZ LLC | 2023 – Present</p>
      <p class="exp-desc">Spearheading end-to-end business operations and wholesale trade, mastering the logistics of high-stakes Dubai commerce.</p>
    </div>

    <div class="exp-item">
      <p class="exp-title">Leadership Portfolio</p>
      <p class="exp-company">2016 – 2023</p>
      <p class="exp-desc">Significant roles in Business Partnership and Administration at Al Marzaan and Anjuman E Najmi, focusing on customer satisfaction and organizational excellence.</p>
    </div>

    <div style="background: #0a192f; color: white; padding: 20px; border-radius: 12px; font-style: italic; text-align: center; font-size: 0.95em;">
      "My commitment to community service defines my professional ethics: Empathy, Responsibility, and Impact."
    </div>
  </div>

  <div class="footer">
    <a href="mailto:tbetwala29@gmail.com" class="cta-btn">CONSULT WITH ME</a>
    <div class="contact-info">
      <strong>📞 Phone:</strong> +971 58 113 0453<br>
      <strong>💬 WhatsApp:</strong> +971 52 179 0412<br>
      <strong>✉️ Email:</strong> tbetwala29@gmail.com
    </div>
    <p style="font-size: 0.75em; color: #999; margin-top: 20px;">© 2026 | Professional Property Services</p>
  </div>
</div>

</body>
</html>

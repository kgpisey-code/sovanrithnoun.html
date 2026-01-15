<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Noun Sovanrith | CV</title>

<link rel="icon" href="cv_1.jpg" />

<style>
/* ===== RESET ===== */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* ===== GLOBAL ===== */
body {
  font-family: "Inter", system-ui, sans-serif;
  background: #f4f5f7;
  color: #111;
  line-height: 1.6;
}

section {
  padding: 90px 20px;
  max-width: 1100px;
  margin: auto;
}

h1, h2, h3 {
  font-weight: 700;
}

h2 {
  text-align: center;
  margin-bottom: 50px;
  font-size: 32px;
}

/* ===== NAVBAR ===== */
.navbar {
  position: fixed;
  top: 12px;
  left: 50%;
  transform: translateX(-50%);
  background: rgba(255, 255, 255, 0.9);
  backdrop-filter: blur(12px);
  padding: 8px 18px;
  border-radius: 40px;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.1);
  z-index: 999;
  max-width: 95%;
  overflow-x: auto;
}

/* Remove scrollbar (mobile) */
.navbar::-webkit-scrollbar {
  display: none;
}

/* Menu */
.navbar ul {
  display: flex;
  gap: 16px;
  list-style: none;
  white-space: nowrap;
}

/* Links */
.navbar a {
  text-decoration: none;
  color: #333;
  font-weight: 500;
  font-size: 14px;
  padding: 6px 10px;
  border-radius: 20px;
  transition: all 0.3s ease;
}

/* Active link */
.navbar a.active {
  font-weight: 700;
  color: #000;
  background: rgba(0, 0, 0, 0.05);
}

/* Hover (desktop only) */
@media (hover: hover) {
  .navbar a:hover {
    background: rgba(0, 0, 0, 0.07);
  }
}

/* ===== MOBILE OPTIMIZATION ===== */
@media (max-width: 768px) {
  .navbar {
    top: 8px;
    padding: 6px 14px;
  }

  .navbar a {
    font-size: 13px;
    padding: 5px 8px;
  }
}


/* ===== HERO ===== */
#home {
  text-align: center;
  padding-top: 140px;
}

#home h1 {
  font-size: 46px;
}

#home p {
  font-size: 20px;
  color: #555;
  margin-top: 10px;
}

.social {
  margin-top: 30px;
}

.social img {
  width: 42px;
  height: 42px;
  border-radius: 50%;
  margin: 0 10px;
  transition: transform 0.3s;
}

.social img:hover {
  transform: scale(1.1);
}

/* ===== ABOUT ===== */
.about-img {
  display: block;
  max-width: 260px;
  margin: 0 auto 30px;
  border-radius: 16px;
}

.about-text {
  max-width: 700px;
  margin: auto;
  text-align: center;
  color: #444;
}

/* ===== PROJECTS ===== */
.project-card {
  display: flex;
  gap: 30px;
  margin-bottom: 30px;
  background: #fff;
  padding: 25px;
  border-radius: 18px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.08);
  transition: transform 0.3s;
}

.project-card:hover {
  transform: translateY(-6px);
}

.project-card img {
  max-width: 320px;
  border-radius: 14px;
}

.tech-stack {
  margin-top: 15px;
  display: flex;
  gap: 10px;
  flex-wrap: wrap;
}

.tech {
  background: #111;
  color: #fff;
  padding: 6px 14px;
  border-radius: 20px;
  font-size: 13px;
}

/* ===== SKILLS ===== */
.skills-grid {
  display: flex;
  gap: 20px;
  justify-content: center;
  flex-wrap: wrap;
}

.skill {
  background: #111;
  color: #fff;
  padding: 12px 22px;
  border-radius: 30px;
  transition: transform 0.3s;
}

.skill:hover {
  transform: scale(1.05);
}

/* ===== EXPERIENCE ===== */
.timeline {
  display: flex;
  flex-direction: column;
  gap: 30px;
}

.timeline-item {
  background: #fff;
  padding: 25px;
  border-radius: 18px;
  box-shadow: 0 8px 25px rgba(0,0,0,0.08);
}

.timeline-item span {
  font-size: 13px;
  color: #777;
}

/* ===== CONTACT ===== */
#contact {
  text-align: center;
  margin-bottom: 5px;
}

.contact-form {
  max-width: 450px;
  margin: auto;
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.contact-form input,
.contact-form textarea {
  padding: 14px;
  border-radius: 10px;
  border: 1px solid #ccc;
}

.contact-form button {
  background: #000;
  color: #fff;
  padding: 14px;
  border-radius: 10px;
  border: none;
  cursor: pointer;
}

/* ===== FOOTER ===== */
footer {
  margin-top: 60px;
  text-align: center;
  font-size: 13px;
  color: #777;
}
/* Skill badge container */
.skill-item {
  position: relative;       /* Needed for dropdown positioning */
  display: inline-block;
  margin: 10px;
}

/* The visible badge */
.skills {
  background: #111;         /* dark badge */
  color: #fff;
  padding: 10px 18px;
  border-radius: 20px;
  font-weight: 500;
  cursor: pointer;
  transition: transform 0.3s;
}

.skills:hover {
  transform: scale(1.05);   /* Slight grow on hover */
}

/* The hidden dropdown content */
.skill-item .dropdown {
  position: absolute;
  top: 130%;               /* dropdown appears below badge */
  left: 50%;
  transform: translateX(-50%);
  background: #fff;
  padding: 12px 16px;
  border-radius: 10px;
  box-shadow: 0 10px 25px rgba(0,0,0,0.2);
  display: flex;
  align-items: center;
  gap: 10px;
  white-space: nowrap;
  opacity: 0;
  visibility: hidden;
  transition: 0.3s ease;
  z-index: 10;
}

/* Image inside dropdown */
.skill-item .dropdown img {
  width: 32px;
  height: 32px;
  border-radius: 6px;
}

/* Show dropdown on hover */
.skill-item:hover .dropdown {
  opacity: 1;
  visibility: visible;
}


/* ===== RESPONSIVE ===== */
@media (max-width: 900px) {
  .project-card {
    flex-direction: column;
    text-align: center;
  }
}
</style>
</head>

<body>

<!-- NAV -->
<nav class="navbar">
  <ul>
    <li><a href="#home" class="nav-link active">Home</a></li>
    <li><a href="#about" class="nav-link">About</a></li>
    <li><a href="#Education" class="nav-link">Education</a></li>
    <li><a href="#skills" class="nav-link">Skills</a></li>
    <li><a href="#experience" class="nav-link">Experience</a></li>
    <li><a href="#contact" class="nav-link">Contact</a></li>
  </ul>
</nav>

<!-- HERO -->
<section id="home">
  <h2></h1>
  <p><strong></string> </p>

  <div class="social">
    <a href="https://www.facebook.com/Sovanrith.Prod/"><img src="facebook1.png"></a>
    <a href="https://t.me/Sovanrithh"><img src="telegram.png"></a>
  </div>
</section>

<!-- ABOUT -->
<section id="about">
  <h2>About Me</h2>
  <img src="picture.jpg" class="about-img">
  <p class="about-text">Name   	 	: 	Noun Sovanrith  </p>
  <p class="about-text">Sex 	 	 	: 	Male   </p>
  <p class="about-text">	Nationality  	 	: 	Cambodian  	   </p>
    <p class="about-text">Marital Status   	: 	Single  </p>
    <p class="about-text"> Date of Birth   	: 	December 16, 1999 </p>
    <p class="about-text">Place of Birth   
 	: 	Samakimeanchey District, Kampong Chhnang Province       </p>
</section>



  <section id="Education" class="project-section">
  <h2 class="section-title">Education</h2>

  <div style="display:flex; gap:20px; flex-wrap:wrap; justify-content:center;">

    <!-- Master's Degree -->
    <div class="project-card" style="flex:1; min-width:260px;">
      <div class="project-text">
        <h3>Present </h3>
        <p> Master’s Degree | Accounting and Auditing </p>
        <p>Norton University – Phnom Penh </p>
      </div>
    </div>

    <!-- Bachelor's Degree -->
    <div class="project-card" style="flex:1; min-width:260px;">
      <div class="project-text">
        <h3>2020</h3>
        <p>Certificate of Bachelor's Degree | Accounting </p>
        <p>Norton University – Phnom Penh </p>
      </div>
    </div>

    <!-- High School -->
    <div class="project-card" style="flex:1; min-width:260px;">
      <div class="project-text">
        <h3>2016</h3>
        <p>Certificate of High School Diploma (General Education)</p>
        <p>	Kampong Tralach High School – Kompong Chhang Province </p>
      </div>
    </div>

  </div>
</section>


</section>

<!-- SKILLS -->
<section id="skills">
  <h2>Skills</h2>
  <div class="skills-grid">

    <!-- English -->
    <div class="skill-item">
      <span class="skills">Khmer</span>
      <div class="dropdown">
        <p>Mother Tongue</p>
      </div>
    </div>

 

    <!-- Database (example from before) -->
    <div class="skill-item">
      <span class="skills">English</span>
      <div class="dropdown">
        <p>Good</p>
      </div>
    </div>

  </div>
</section>


<!-- EXPERIENCE -->
<section id="experience">
  <h2>Work Experience</h2>

  <div class="timeline">

    <!-- 1. Senior Tax Accountant - H.SPC CO., LTD -->
    <div class="timeline-item">
      <span>2024 – Present</span>
      <h3>Senior Tax Accountant</h3>
      <h4>H.SPC CO., LTD. - Phnom Penh</h4>
      <ul>
        <li>Check and verify Payment, Receipt, and Journal Vouchers</li>
        <li>Check inventory listing and help count stock</li>
        <li>Surprise cash check at store</li>
        <li>Train team on accounting and tax law</li>
        <li>Manage company petty cash</li>
        <li>Make payments and solve supplier issues</li>
        <li>Check staff payroll and process payment</li>
        <li>Verify transactions in Sage 50 system</li>
        <li>Prepare and review financial statements</li>
        <li>Prepare monthly and annual tax</li>
        <li>Prepare documents for ministries</li>
        <li>Assist with tax and external audits</li>
        <li>Tax research and guidance for business decisions</li>
        <li>Other tasks assigned by Finance Manager</li>
      </ul>
    </div>

    <!-- 2. Senior Tax Accountant - Compass Advertising Co., Ltd -->
    <div class="timeline-item">
      <span>2023 – Present</span>
      <h3>Senior Tax Accountant</h3>
      <h4>Compass Advertising Co., Ltd. - Phnom Penh</h4>
      <ul>
        <li>Verify and monitor accounting transactions</li>
        <li>Prepare all accounting documents (Payment, Petty Cash, Receipt, Journal Vouchers)</li>
        <li>Post transactions into QuickBooks and reconcile ledger</li>
        <li>Closing monthly and annual accounting reports</li>
        <li>Monthly and annual tax declaration</li>
        <li>Prepare documents for ministries</li>
        <li>Assist with tax audits and objections</li>
        <li>Prepare unaudited reports for regulator</li>
        <li>Other tasks assigned by Finance Manager</li>
      </ul>
    </div>

    <!-- 3. Accounting Assistant - Fides Service (Cambodia) Ltd -->
    <div class="timeline-item">
      <span>2019 – 2023</span>
      <h3>Accounting Assistant</h3>
      <h4>Fides Service (Cambodia) Ltd. - Phnom Penh</h4>
      <ul>
        <li>Closing monthly and annual accounting reports</li>
        <li>Monthly and annual tax declaration</li>
        <li>Assist with tax audit and external audit</li>
        <li>Prepare unaudited report for ACAR</li>
        <li>Other tasks assigned by manager</li>
      </ul>
    </div>

    <!-- 4. AP Accounting Assistant - ALIS International School -->
    <div class="timeline-item">
      <span>2018 – 2019</span>
      <h3>AP Accounting Assistant</h3>
      <h4>ALIS International School - Phnom Penh</h4>
      <ul>
        <li>Control monthly expenses</li>
        <li>Purchase materials for mechanics</li>
        <li>Solve vendor problems</li>
        <li>Prepare monthly reports for manager</li>
      </ul>
    </div>

    <!-- 5. Teacher Assistant - ALIS International School -->
    <div class="timeline-item">
      <span>2017 – 2018</span>
      <h3>Teacher Assistant</h3>
      <h4>ALIS International School - Phnom Penh</h4>
      <ul>
        <li>Control students in classes</li>
        <li>Prepare documents for teachers</li>
        <li>Teach Khmer language to students</li>
        <li>Prepare lesson plans</li>
      </ul>
    </div>

    <!-- 6. Operation Staff - CLN (Cambodia) Co., Ltd -->
    <div class="timeline-item">
      <span>2016 – 2017</span>
      <h3>Operation Staff</h3>
      <h4>CLN (Cambodia) Co., Ltd – Phnom Penh</h4>
      <ul>
        <li>Check import documents for clients</li>
        <li>Follow up with clients and vendors</li>
        <li>Prepare LOLO processing</li>
        <li>Issue sales invoices</li>
        <li>Other tasks assigned by management</li>
      </ul>
    </div>

  </div>
</section>


<!-- CONTACT -->
<section id="contact">
  <h2>Contact Me</h2>
  <p>Email: Sovanrithnoun1299@gmail.com</p>

  <form class="contact-form" action="mailto:Sovanrithnoun1299@gmail.com" method="post" enctype="text/plain">
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
  <input type="text" name="Name" placeholder="Your Name" required>
  <input type="email" name="Email" placeholder="Your Email" required>
  <textarea name="Message" placeholder="Your Message" required></textarea>
  <button type="submit">Send</button>
</form>

</section>


<footer>
  © 2025 Noun Sovanrith
</footer>

<script>
const links = document.querySelectorAll(".nav-link");
const sections = document.querySelectorAll("section");

window.addEventListener("scroll", () => {
  let current = "";
  sections.forEach(sec => {
    if (pageYOffset >= sec.offsetTop - 200) {
      current = sec.id;
    }
  });

  links.forEach(a => {
    a.classList.remove("active");
    if (a.getAttribute("href") === "#" + current) {
      a.classList.add("active");
    }
  });
});
</script>

</body>
</html>

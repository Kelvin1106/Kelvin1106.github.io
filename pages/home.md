---
layout: default
title: Home
permalink: /
---

<style>
/* Experience Page Specific Styles */

.experience-container {
  max-width: 1300px;
  margin: 3rem auto 0 auto;
  padding: 0 2rem;
  display: grid;
  grid-template-columns: 280px 1fr;
  /* gap: 3rem; */
}

.experience-sidebar {
  background: white;
  border-radius: 12px;
  padding: 2rem;
  height: fit-content;
  position: sticky;
  top: 120px;
}

.sidebar-profile-pic {
  width: 150px;
  height: 150px;
  border-radius: 20%;
  object-fit: cover;
  display: block;
  margin: 0 auto; /* 水平置中 */
}

.sidebar-profile-name {
  font-size: 1.1rem;
  font-weight: 600;
  margin-bottom: 0.5rem;
  color: #2c3e50;
  font-family: 'Georgia', 'Times New Roman', serif;
}

.sidebar-profile-title {
  color: #666;
  margin-bottom: 2rem;
  font-size: 0.95rem;
  line-height: 1.5;
}

.sidebar-contact-info {
  list-style: none;
  padding: 0;
}

.sidebar-contact-info li {
  margin-bottom: 0.8rem;
  font-size: 0.9rem;
  color: #666;
}

.sidebar-contact-info i {
  width: 20px;
  margin-right: 0.5rem;
  color: #666;
}

.sidebar-contact-info a {
  color: #666;
  text-decoration: none;
}

.sidebar-contact-info a:hover {
  text-decoration: underline;
}

.experience-content {
  background: white;
  border-radius: 12px;
}

.experience-content-header {
  background: #6c757d;
  color: white;
  padding: 1.5rem 2rem;
  border-radius: 12px 12px 0 0;
}

.experience-section-nav {
  background: #f8f9fa;
  padding: 1rem 2rem;
  border-bottom: 1px solid #e9ecef;
}

.experience-section-nav ul {
  list-style: none;
  display: flex;
  gap: 2rem;
  margin: 0;
  padding: 0;
}

.experience-section-nav a {
  text-decoration: none;
  color: #666;
  font-weight: 500;
  padding: 0.5rem 0;
  border-bottom: 2px solid transparent;
  transition: all 0.3s ease;
}

.experience-section-nav a.active {
  color: #007bff;
  border-bottom-color: #007bff;
}

.experience-section-title {
  font-size: 1.8rem;
  font-weight: 600;
  margin-bottom: 1rem;
  color: #2c3e50;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid #0a0100ff;
}

.experience-item {
  margin-bottom: 3rem;
  border-bottom: 1px solid #e9ecef;
}

.experience-item:last-child {
  border-bottom: none;
  margin-bottom: 0;
}

.experience-header {
  margin-bottom: 1rem;
}

.position-title {
  color: #007bff;
  font-weight: 600;
  font-size: 1.2rem;
  margin-bottom: 0.5rem;
}

.company-info {
  color: #666;
  font-style: italic;
  margin-bottom: 0.5rem;
}

.duration {
  color: #28a745;
  font-weight: 500;
  font-size: 0.9rem;
}

.experience-description {
  color: #555;
  line-height: 1.6;
}

ul {
    padding-left: 20px; /* 保持縮排 */
    margin: 0; /* 拿掉不必要的上下外距 */
}

.experience-description ul {
  margin-left: 1.5rem;
  margin-top: 0.5rem;
}

.experience-description li {
  margin-bottom: 0.5rem;
}

/* Responsive Design */
@media (max-width: 768px) {
  .experience-container {
    grid-template-columns: 1fr;
    gap: 2rem;
  }

  .experience-sidebar {
    position: static;
  }

  .hero-title {
    font-size: 2rem;
  }

  .experience-section-nav ul {
    flex-direction: column;
    gap: 0.5rem;
  }
}
</style>

<!-- Main Container -->
<div class="experience-container">
  <!-- Sidebar -->
  <aside class="experience-sidebar">
    <img src="{{ site.baseurl }}/assets/img/profile.png" alt="Profile photo" class="sidebar-profile-pic">
    <h3 class="sidebar-profile-name">Chia-Yi (Charlie) Chin</h3>
    <ul class="sidebar-contact-info">
      <li><i class="fa-solid fa-building"></i> {{ site.author.employer }}</li>
      <li><i class="fa-solid fa-location-dot"></i> {{ site.author.location }}</li>
      <li><i class="fa-solid fa-envelope"></i> <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a></li>
      <li><i class="fa-brands fa-github"></i> <a href="https://github.com/{{ site.author.github }}">GitHub</a></li>
      <li><i class="fa-brands fa-linkedin"></i> <a href="{{ site.author.linkedin }}">LinkedIn</a></li>
    </ul>
  </aside>

  <!-- Main Content -->
  <main class="experience-content">
    <div>
        <section id="research">
            <h3 class="experience-section-title">About Me</h3>
            <p>
            Hello! 👋 My name is Chia-Yi (Charlie) Chin. I am currently an undergraduate student 
            in the Department of Electrical Engineering at National Taiwan University, 
            expecting to graduate in January 2026. 
            My research interests include 
            <strong>Hardware & Software Co-Design for ML Accelerators</strong>, 
            <strong>ASIC/FPGA VLSI Circuit Design</strong>, and 
            <strong>Distributed Computing for LLM Systems</strong>.
            </p>
            <p>
            For detailed information:
            <a href="assets/CV-Charlie.pdf" 
                target="_blank" 
                rel="noopener"
                style="color:#006666; font-weight:bold; text-decoration:none;"
                onmouseover="this.style.textDecoration='underline';"
                onmouseout="this.style.textDecoration='none';">
                📄 CV (as of August, 2025)
            </a>
            </p>
            <h3 class="experience-section-title">Recent News</h3>
            <p>
            🏆 Jun 2025 – Accepted as a participant in 
            <a href="https://sc25.supercomputing.org/students/student-cluster-competition/" 
                style="color:#006666; font-weight:bold; font-style:italic; text-decoration:none;"
                onmouseover="this.style.textDecoration='underline';"
                onmouseout="this.style.textDecoration='none';">
                Student Cluster Final Competition (SCC25)
            </a>, St. Louis, USA !
            </p>
            <p>
            🏆 Jun 2025 – Accepted as a participant in 
            <a href="https://www.hpcadvisorycouncil.com/events/2025/APAC-AI-HPC/" 
                style="color:#006666; font-weight:bold; font-style:italic; text-decoration:none;"
                onmouseover="this.style.textDecoration='underline';"
                onmouseout="this.style.textDecoration='none';">
                2025 APAC HPC-AI Competition
            </a>!
            </p>
            <p>
            🏆 May 2025 – Accepted as a participant in 
            <a href="https://www.asc-events.net/StudentChallenge/ASC25/Register.php" 
                style="color:#006666; font-weight:bold; font-style:italic; text-decoration:none;"
                onmouseover="this.style.textDecoration='underline';"
                onmouseout="this.style.textDecoration='none';">
                Supercomputer Challenge Final Competition (ASC25)
            </a>, Qinghai, China !
            </p>
            <h3 class="experience-section-title">Education</h3>
            <ul>
                <li>
                    <strong>B.S. at National Taiwan University, Taiwan</strong>
                    <ul>
                        <li>Electrical Engineering, 2022 – 2026 (expected)</li>
                        <li>Mechanical Engineering, 2021 – 2022 (transferred tracks)</li>
                    </ul>
                </li>
            </ul>
        </section>
        </div>
  </main>
</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const navLinks = document.querySelectorAll('.experience-section-nav a');
  
  navLinks.forEach(link => {
    link.addEventListener('click', function(e) {
      e.preventDefault();
      
      // Remove active class from all links
      navLinks.forEach(l => l.classList.remove('active'));
      
      // Add active class to clicked link
      this.classList.add('active');
      
      // You can add section switching logic here
      console.log('Switched to:', this.getAttribute('href'));
    });
  });
});
</script>
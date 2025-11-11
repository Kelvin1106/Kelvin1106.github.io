---
layout: default
title: Home
permalink: /
---

<style>
/* Experience Page Specific Styles */

  .sidebar-contact-info li {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.sidebar-contact-info a {
  white-space: nowrap;          /* 不換行 */
  overflow: hidden;             /* 超出就截斷 */
  text-overflow: ellipsis;      /* 加省略號 */
  min-width: 0;                 /* flex 裡讓省略號生效 */
  display: inline-block;
}
.experience-container {
  max-width: 1300px;
  margin: 3rem auto 0 auto;
  padding: 0 2rem;
  display: grid;
  grid-template-columns: 320px minmax(0,1fr);  /* 280px → 360px（可再調大） */
  column-gap: 2.5rem;
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
  display: flex;
  align-items: center;
  gap: 0.6rem;
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
    <h3 class="sidebar-profile-name">Kai-Hua (Kelvin) Wang</h3>
    <ul class="sidebar-contact-info">
      <li><i class="fa-solid fa-building"></i> {{ site.author.employer }}</li>
      <li><i class="fa-solid fa-location-dot"></i> {{ site.author.location }}</li>
      <li><i class="fa-solid fa-envelope"></i> <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a></li>
      <li><i class="fa-brands fa-linkedin"></i> <a href="{{ site.author.linkedin }}">LinkedIn</a></li>
      <li><i class="fa-brands fa-github"></i> <a href="https://github.com/{{ site.author.github }}">GitHub</a></li>
    </ul>
  </aside>

  <!-- Main Content -->
  <main class="experience-content">
    <div>
        <section id="research">
            <h3 class="experience-section-title">About Me</h3>
            <p>
            Hello! 👋 My name is Kai-Hua (Kelvin) Wang. I am currently an undergraduate student 
            in the Department of Mechanical Engineering at National Taiwan University, 
            expecting to graduate in January 2026. 
            My research interests include 
            <strong>Robotics, sensing, and localization</strong>, 
            <strong>Vehicle dynamics and modeling</strong>, and 
            <strong>Medical devices and prototyping</strong>.
            </p>
            <p>
            For detailed information:
            <a href="assets/Kai_Hua_Wang_s_CV.pdf" 
                target="_blank" 
                rel="noopener"
                style="color:#006666; font-weight:bold; text-decoration:none;"
                onmouseover="this.style.textDecoration='underline';"
                onmouseout="this.style.textDecoration='none';">
                📄 CV (as of October, 2025)
            </a>
            </p>
            <h3 class="experience-section-title">Awards and Honors</h3>
            <p>
            🏆 Jul 2023 -
            <a href="https://www.fstaiwan.net/" 
                style="color:#006666; font-weight:bold; font-style:italic; text-decoration:none;"
                onmouseover="this.style.textDecoration='underline';"
                onmouseout="this.style.textDecoration='none';">
                Formula Student Taiwan
            </a>1st Overall as <strong>Aerodynamics Lead</strong> !
            </p>
            <p>
            🥈 Aug 2022 - 
            <a href="https://www.fstaiwan.net/" 
                style="color:#006666; font-weight:bold; font-style:italic; text-decoration:none;"
                onmouseover="this.style.textDecoration='underline';"
                onmouseout="this.style.textDecoration='none';">
                Formula Student Taiwan
            </a>2nd Overall !
            </p>
            <h3 class="experience-section-title">Education</h3>
            <ul>
                <li>
                    <strong>B.S. at National Taiwan University, Taiwan</strong>
                    <ul>
                        <li>Mechanical Engineering, 2021 – 2026 (Expected)</li>
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







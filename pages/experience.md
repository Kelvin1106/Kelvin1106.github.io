---
layout: default
title: Experience
permalink: /experience/
---

<style>
/* Experience Page Monochrome Styles */

body {
  background-color: #F8F9FA;
  color: #2D3748;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  margin: 0;
}

.experience-container {
  max-width: 1200px;
  margin: 3rem auto 0 auto;
  padding: 0 2rem;
  display: grid;
  grid-template-columns: 300px minmax(0, 1fr);
  column-gap: 2.5rem;
}

/* 側邊欄卡片化 */
.experience-sidebar {
  background: #FFFFFF;
  border-radius: 10px;
  padding: 2rem;
  height: fit-content;
  position: sticky;
  top: 120px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.03);
  border: 1px solid rgba(226, 232, 240, 0.8);
}

.sidebar-profile-pic {
  width: 180px;
  height: 180px;
  border-radius: 12px;
  object-fit: cover;
  display: block;
  margin: 0 auto 1.5rem auto;
  border: 3px solid #F8F9FA;
}

.sidebar-profile-name {
  font-size: 1.25rem;
  font-weight: 800;
  margin-bottom: 0.25rem;
  color: #1A202C;
  letter-spacing: -0.02em;
  text-align: center;
}

.sidebar-profile-title {
  color: #718096;
  margin-bottom: 2rem;
  font-size: 0.9rem;
  line-height: 1.5;
  text-align: center;
  font-weight: 500;
}

.sidebar-contact-info {
  list-style: none;
  padding: 0;
  margin: 0;
}

.sidebar-contact-info li {
  display: flex;
  align-items: center;
  gap: 0.6rem;
  margin-bottom: 0.8rem;
  font-size: 0.9rem;
  color: #4A5568;
}

.sidebar-contact-info i {
  width: 20px;
  color: #718096;
}

.sidebar-contact-info a {
  color: #4A5568;
  text-decoration: none;
  transition: color 0.2s ease;
}

.sidebar-contact-info a:hover {
  color: #1A202C;
  text-decoration: underline;
}

/* 主內容區 */
.experience-content {
  background: #FFFFFF;
  border-radius: 10px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.03);
  border: 1px solid rgba(226, 232, 240, 0.8);
  overflow: hidden;
}

.experience-content-header {
  background: #1A202C; /* 沉穩極簡黑 */
  color: #FFFFFF;
  padding: 1.5rem 2.5rem;
}

.experience-content-header h2 {
  margin: 0;
  font-size: 1.3rem;
  font-weight: 800;
  letter-spacing: -0.01em;
  display: flex;
  align-items: center;
  gap: 0.75rem;
}

.experience-body {
  padding: 2.5rem;
}

.experience-section-title {
  font-size: 1.3rem;
  font-weight: 800;
  margin-bottom: 1.5rem;
  margin-top: 2.5rem;
  color: #1A202C;
  padding-bottom: 0.5rem;
  border-bottom: 1px solid #E2E8F0;
  letter-spacing: -0.01em;
}

.experience-section-title:first-of-type {
  margin-top: 0;
}

/* Experience Items Typography */
.experience-item {
  margin-bottom: 2rem;
  padding-bottom: 1.5rem;
  border-bottom: 1px solid #F1F5F9;
}

.experience-item:last-child {
  border-bottom: none;
  margin-bottom: 0;
  padding-bottom: 0;
}

.experience-header {
  margin-bottom: 0.75rem;
}

.position-title {
  color: #1A202C;
  font-weight: 800;
  font-size: 1.1rem;
  margin: 0 0 0.25rem 0;
  letter-spacing: -0.01em;
}

.company-info {
  color: #4A5568;
  font-weight: 500;
  font-size: 0.95rem;
  margin: 0 0 0.25rem 0;
}

.duration {
  color: #718096;
  font-weight: 600;
  font-size: 0.85rem;
  margin: 0;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

/* 經典極簡 Bullet Points */
.experience-description ul {
  padding-left: 1.2rem;
  margin: 0.5rem 0 0 0;
  list-style-type: disc;
}

.experience-description li {
  margin-bottom: 0.4rem;
  color: #4A5568;
  line-height: 1.6;
  font-size: 0.95rem;
}

/* Responsive Design */
@media (max-width: 768px) {
  .experience-container {
    grid-template-columns: 1fr;
    gap: 1.5rem;
    padding: 0 1rem;
  }

  .experience-sidebar {
    position: static;
  }

  .experience-body {
    padding: 1.5rem;
  }
}
</style>

<!-- Main Container -->
<div class="experience-container">
  <!-- Sidebar -->
  <aside class="experience-sidebar">
    <img src="{{ site.baseurl }}/assets/profile.png" alt="Profile photo" class="sidebar-profile-pic">
    <h3 class="sidebar-profile-name">Kai-Hua (Kelvin) Wang</h3>
    <p class="sidebar-profile-title">M.S. Student @ CMU ME</p>
    <ul class="sidebar-contact-info">
      <li><i class="fa-solid fa-building"></i> {{ site.author.employer }}</li>
      <li><i class="fa-solid fa-location-dot"></i> {{ site.author.location }}</li>
      <li><i class="fa-solid fa-envelope"></i> <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a></li>
      <li><i class="fa-brands fa-linkedin"></i> <a href="{{ site.author.linkedin }}">LinkedIn</a></li>
    </ul>
  </aside>

  <!-- Main Content -->
  <main class="experience-content">
    <div class="experience-content-header">
      <h2><i class="fa-solid fa-briefcase"></i> Experience</h2>
    </div>

    <div class="experience-body">
      <!-- Research Experience Section -->
      <h3 class="experience-section-title">Research Experience</h3>

      <div class="experience-item">
        <div class="experience-header">
          <h4 class="position-title">System Optimization Laboratory, National Taiwan University</h4>
          <p class="company-info">Undergraduate Researcher (Advisor: Prof. Kuei-Yuan Chan)</p>
          <p class="duration">Sep. 2024 – Present</p>
        </div>
        <div class="experience-description">
          <ul>
            <li><strong>Scaled Autonomous Straddle Carrier:</strong> Developed a 1:14 scaled experimental platform for container terminal operations and trajectory studies.</li>
            <li><strong>Foxtron Vehicle Technologies Collaboration:</strong> Industry-academia partnership focusing on vehicle dynamics and control modeling.</li>
          </ul>
        </div>
      </div>

      <div class="experience-item">
        <div class="experience-header">
          <h4 class="position-title">Smart and Advanced Manufacturing Laboratory, National Taiwan University</h4>
          <p class="company-info">Undergraduate Researcher (Advisor: Prof. Dian-Ru Li)</p>
          <p class="duration">Oct. 2022 – Present</p>
        </div>
        <div class="experience-description">
          <ul>
            <li><strong>Double Lumen Catheter Stabilizer:</strong> Collaborated with Taipei Medical University on medical device prototyping and validation.</li>
          </ul>
        </div>
      </div>

      <div class="experience-item">
        <div class="experience-header">
          <h4 class="position-title">NTU Racing (Formula SAE), National Taiwan University</h4>
          <p class="company-info">Aerodynamics Team Lead</p>
          <p class="duration">Jul. 2022 – Jul. 2023</p>
        </div>
        <div class="experience-description">
          <ul>
            <li>Led a 7-person engineering team to design, simulate, and manufacture high-performance carbon fiber aero kits.</li>
          </ul>
        </div>
      </div>

      <!-- Working Experience Section -->
      <h3 class="experience-section-title">Working Experience</h3>

      <div class="experience-item">
        <div class="experience-header">
          <h4 class="position-title">Garmin Corporation</h4>
          <p class="company-info">NPI Engineer Intern</p>
          <p class="duration">Jul. 2024 – Jan. 2025</p>
        </div>
        <div class="experience-description">
          <ul>
            <li><strong>Pressing Process Standardization:</strong> Standardized assembly processes for handheld device displays to meet IPX7 waterproof standards.</li>
            <li><strong>GPSMAP Accessory Development:</strong> Executed manufacturing process design using Therblig analysis, PFMEA, and custom fixture development.</li>
          </ul>
        </div>
      </div>

      <!-- Teaching Experience Section -->
      <h3 class="experience-section-title">Teaching Experience</h3>

      <div class="experience-item">
        <div class="experience-header">
          <h4 class="position-title">Teaching Assistant, National Taiwan University</h4>
          <p class="company-info">Department of Mechanical Engineering</p>
        </div>
        <div class="experience-description">
          <ul>
            <li><strong>ME5024: Design and Practice of Intelligent Vehicles (I)</strong> — Fall 2025</li>
            <li><strong>ME5025: Design and Practice of Intelligent Vehicles (II)</strong> — Spring 2024</li>
          </ul>
        </div>
      </div>

    </div>
  </main>
</div>

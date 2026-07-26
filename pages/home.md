---
layout: default
title: Home
permalink: /
---

<style>
/* Base Background & Typography Optimization */
body {
  background-color: #F4F6F8;
  color: #2D3748;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  margin: 0;
}

/* Experience Page Specific Styles */
.sidebar-contact-info li {
  display: flex;
  align-items: center;
  gap: 0.6rem;
  margin-bottom: 0.8rem;
  font-size: 0.9rem;
  color: #4A5568;
}

.sidebar-contact-info a {
  white-space: nowrap;          /* 不換行 */
  overflow: hidden;             /* 超出就截斷 */
  text-overflow: ellipsis;      /* 加省略號 */
  min-width: 0;                 /* flex 裡讓省略號生效 */
  display: inline-block;
  color: #4A5568;
  text-decoration: none;
  transition: color 0.2s ease;
}

.sidebar-contact-info a:hover {
  color: #FF4D00;               /* 大迫傑/運動感 鮮明橘色點綴 */
  text-decoration: none;
}

.sidebar-contact-info i {
  width: 20px;
  color: #718096;
}

.experience-container {
  max-width: 1200px;
  margin: 3rem auto 0 auto;
  padding: 0 2rem;
  display: grid;
  grid-template-columns: 300px minmax(0, 1fr);
  column-gap: 2.5rem;
}

/* 側邊欄卡片化（俐落圓角與懸浮陰影） */
.experience-sidebar {
  background: #FFFFFF;
  border-radius: 10px;
  padding: 2rem;
  height: fit-content;
  position: sticky;
  top: 120px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.04);
  border: 1px solid rgba(226, 232, 240, 0.8);
}

.sidebar-profile-pic {
  width: 180px;
  height: 180px;
  border-radius: 12px;           /* 改為俐落的極簡方圓形 */
  object-fit: cover;
  display: block;
  margin: 0 auto 1.5rem auto;
  border: 3px solid #F4F6F8;
}

.sidebar-profile-name {
  font-size: 1.25rem;
  font-weight: 700;
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
  font-weight: 400;
}

.sidebar-contact-info {
  list-style: none;
  padding: 0;
  margin: 0;
}

/* 主內容區卡片化 */
.experience-content {
  background: #FFFFFF;
  border-radius: 10px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.04);
  border: 1px solid rgba(226, 232, 240, 0.8);
  overflow: hidden;
  padding: 2.5rem;
}

.experience-section-nav {
  background: #FFFFFF;
  padding: 0;
  border-bottom: 1px solid #E2E8F0;
  margin-bottom: 2rem;
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
  color: #718096;
  font-weight: 600;
  font-size: 0.95rem;
  padding: 0.75rem 0;
  display: inline-block;
  border-bottom: 3px solid transparent;
  transition: all 0.2s ease;
}

.experience-section-nav a.active,
.experience-section-nav a:hover {
  color: #1A202C;
  border-bottom-color: #FF4D00; /* 加厚競技橘色底線 */
  font-weight: 700;
}

/* Section Body Settings */
.experience-section-title {
  font-size: 1.5rem;
  font-weight: 700;
  margin-bottom: 1.25rem;
  margin-top: 2rem;
  color: #1A202C;
  padding-bottom: 0.5rem;
  border-bottom: 1px solid #E2E8F0;
  letter-spacing: -0.01em;
}

.experience-section-title:first-of-type {
  margin-top: 0;
}

/* 清單與自訂點綴符號 */
ul {
  padding-left: 0;
  margin: 0;
  list-style: none;
}

ul li {
  position: relative;
  padding-left: 1.2rem;
  margin-bottom: 0.5rem;
  color: #4A5568;
  line-height: 1.7;
}

ul li::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0.65em;
  width: 5px;
  height: 5px;
  background-color: #FF4D00;   /* 自訂亮橘小矩形點綴 */
  border-radius: 1px;
}

/* 內層 nested ul 不重複疊加樣式 */
ul ul {
  margin-top: 0.25rem;
}

ul ul li::before {
  background-color: #A0AEC0;   /* 第二層點點改為質感灰色 */
}

/* Resume Button Styling */
.cv-btn-container {
  margin-top: 1.5rem;
  margin-bottom: 2rem;
}

.cv-button {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  background-color: #1A202C;
  color: #FFFFFF !important;
  padding: 0.65rem 1.25rem;
  border-radius: 6px;
  font-weight: 600;
  font-size: 0.9rem;
  text-decoration: none !important;
  transition: all 0.2s ease-in-out;
  box-shadow: 0 2px 4px rgba(0,0,0,0.08);
}

.cv-button:hover {
  background-color: #FF4D00;
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(255, 77, 0, 0.25);
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

  .experience-section-nav ul {
    flex-direction: column;
    gap: 0;
  }

  .experience-section-nav a {
    padding: 0.75rem 0;
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
    <section id="about">
      <!-- About Me Section -->
      <h3 class="experience-section-title">About Me</h3>
      <p style="line-height: 1.7; color: #4A5568;">
        Hello! I'm <strong>Kai-Hua (Kelvin) Wang</strong>, an incoming M.S. student in Mechanical Engineering (Research Track) at <strong>Carnegie Mellon University</strong>, where I conduct research in the <strong>TRIO Lab</strong>. I hold a B.S. in Mechanical Engineering from <strong>National Taiwan University</strong>.
      </p>
      <p style="line-height: 1.7; color: #4A5568;">
        My research focuses on <strong>control theory, optimization, and robotics</strong> to build safe, agile, and intelligent autonomous systems.
      </p>
      <p style="margin-top: 1rem; font-weight: 700; color: #1A202C;">Research Interests:</p>
      <ul>
        <li><strong>Safe & Agile Autonomous Systems:</strong> Safety-critical planning and human-aware autonomy</li>
        <li><strong>Dynamics & Control:</strong> State estimation and learning-enhanced modeling for physical platforms</li>
      </ul>
      <p style="line-height: 1.7; color: #4A5568; margin-top: 1rem;">
        Outside the lab, I am an active marathon runner and endurance sports enthusiast. I bring the same discipline and persistence from the track to my engineering research.
      </p>
      
      <!-- Resume Button -->
      <div class="cv-btn-container">
        <a href="{{ site.baseurl }}/assets/Kai_Hua_Wang_s_CV.pdf" 
           target="_blank" 
           rel="noopener noreferrer"
           class="cv-button">
          <i class="fa-solid fa-file-pdf"></i> View Full Resume (PDF)
        </a>
      </div>

      <!-- Education Section -->
      <h3 class="experience-section-title">Education</h3>
      <ul>
        <li>
          <strong>Carnegie Mellon University</strong> — M.S. in Mechanical Engineering
          <ul>
            <li>Pittsburgh, PA, USA | Aug. 2026 – May 2028 (Expected)</li>
          </ul>
        </li>
        <li>
          <strong>National Taiwan University</strong> — B.S. in Mechanical Engineering
          <ul>
            <li>Taipei, Taiwan | Sep. 2021 – Jan. 2026</li>
          </ul>
        </li>
      </ul>

      <!-- Awards and Honors Section -->
      <h3 class="experience-section-title">Awards and Honors</h3>
      <p style="line-height: 1.7; color: #4A5568;">
        🏆 Jul 2023 - 
        <a href="https://www.fstaiwan.net/" 
           target="_blank"
           rel="noopener"
           style="color:#FF4D00; font-weight:bold; font-style:italic; text-decoration:none;">
          Formula Student Taiwan
        </a> 
        1st Overall as <strong>Aerodynamics Lead</strong>!
      </p>
      <p style="line-height: 1.7; color: #4A5568;">
        🥈 Aug 2022 - 
        <a href="https://www.fstaiwan.net/" 
           target="_blank"
           rel="noopener"
           style="color:#FF4D00; font-weight:bold; font-style:italic; text-decoration:none;">
          Formula Student Taiwan
        </a> 
        2nd Overall!
      </p>
    </section>
  </main>
</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const navLinks = document.querySelectorAll('.experience-section-nav a');
  
  navLinks.forEach(link => {
    link.addEventListener('click', function(e) {
      e.preventDefault();
      
      navLinks.forEach(l => l.classList.remove('active'));
      this.classList.add('active');
      
      console.log('Switched to:', this.getAttribute('href'));
    });
  });
});
</script>

---
layout: default
title: Beyond
permalink: /beyond/
---

<style>
/* Beyond Page Monochrome Styles - Refined Sharpness */

body {
  background-color: #F8F9FA;
  color: #2D3748;
  font-family: "Inter", -apple-system, BlinkMacSystemFont, "SF Pro Text", "Segoe UI", Roboto, sans-serif;
  margin: 0;
  -webkit-font-smoothing: antialiasing;
  -moz-osx-font-smoothing: grayscale;
}

.experience-container {
  max-width: 1200px;
  margin: 3rem auto 0 auto;
  padding: 0 2rem;
  display: grid;
  grid-template-columns: 300px minmax(0, 1fr);
  column-gap: 2.5rem;
}

/* 側邊欄卡片化（完全對齊 home & experience） */
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
  object-position: center 20%;
  display: block;
  margin: 0 auto 1.5rem auto;
  border: 3px solid #F8F9FA;
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
  font-weight: 500;
  letter-spacing: 0.01em;
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
  padding: 1.25rem 2.5rem;
}

.experience-content-header h2 {
  margin: 0;
  font-size: 1.2rem;
  font-weight: 700;
  letter-spacing: -0.01em;
  display: flex;
  align-items: center;
  gap: 0.75rem;
}

.experience-body {
  padding: 2.5rem;
}

.experience-section-title {
  font-size: 1.25rem;
  font-weight: 700;
  margin-bottom: 1.5rem;
  margin-top: 2.5rem;
  color: #1A202C;
  padding-bottom: 0.5rem;
  border-bottom: 1px solid #E2E8F0;
  letter-spacing: -0.02em;
}

.experience-section-title:first-of-type {
  margin-top: 0;
}

/* Beyond Page Specific Items */
.beyond-item {
  margin-bottom: 2rem;
  padding-bottom: 1.5rem;
  border-bottom: 1px solid #F1F5F9;
}

.beyond-item:last-child {
  border-bottom: none;
  margin-bottom: 0;
  padding-bottom: 0;
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
      <h2><i class="fa-solid fa-compass"></i> Beyond the Lab</h2>
    </div>

    <div class="experience-body">
      <!-- Hobbies & Interests Section -->
      <h3 class="experience-section-title">Endurance & Marathon</h3>
      
      <p style="line-height: 1.7; color: #4A5568;">
        To be updated...
      </p>

    </div>
  </main>
</div>

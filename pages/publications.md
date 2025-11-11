---
layout: default
title: Publications
permalink: /publications/
---

<style>
/* Page Styles (沿用你的版型) */
.experience-container {
  max-width: 1300px;
  margin: 3rem auto 0 auto;
  padding: 0 2rem;
  display: grid;
  grid-template-columns: 300px 1fr;
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
  margin: 0 auto;
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

.experience-section-title {
  font-size: 1.8rem;
  font-weight: 600;
  margin: 2rem 0 1rem 0;
  color: #2c3e50;
  border-bottom: 2px solid #0a0100ff;
  padding-bottom: 0.4rem;
}

.pub-list {
  padding-left: 1.2rem;
  margin: 0;
  font-size: 1.05rem;
}

.pub-list li { 
  margin: 0 0 0.9rem 0;
  line-height: 1.55;
}

.pub-title { font-weight: 600; }
.pub-venue { font-style: italic; color:#555; }
.pub-badge {
  display: inline-block;
  font-size: 0.75rem;
  padding: 0.15rem 0.5rem;
  border-radius: 999px;
  border: 1px solid #cbd3da;
  color: #6c757d;
  vertical-align: middle;
  margin-left: 0.4rem;
}

/* Responsive */
@media (max-width: 768px) {
  .experience-container { grid-template-columns: 1fr; gap: 2rem; }
  .experience-sidebar { position: static; }
}
</style>

<div class="experience-container">
  <!-- Sidebar -->
  <aside class="experience-sidebar">
    <img src="{{ site.baseurl }}/assets/img/profile.png" alt="Profile photo" class="sidebar-profile-pic">
    <h3 class="sidebar-profile-name">Kai-Hua (Kelvin) Wang</h3>
    <p class="sidebar-profile-title">
      Robotics for sensing, localization, and trajectory planning ·
      Vehicle dynamics & modeling ·
      Medical device prototyping & validation
    </p>
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
    <div class="experience-content-header">
      <h2><i class="fa-solid fa-book-open"></i> Publications</h2>
    </div>

    <!-- In preparation -->
    <h3 class="experience-section-title">In preparation</h3>
    <ol class="pub-list">
      <li>
        <span class="pub-title">HemoSeal Stabilizer for double-lumen hemodialysis catheter exchange: design and simulator-based evaluation</span>.
        <strong>Kai-Hua, Wang</strong>, <span>et al.</span>
        <span class="pub-venue">Journal manuscript in preparation</span> , Advisor: Dian-Ru Li 
        <span class="pub-badge">medical devices</span>
      </li>
    </ol>

    <!-- 之後要新增 peer-reviewed 或 preprints，可在這裡再加區塊 -->
    <!--
    <h3 class="experience-section-title">Peer-reviewed</h3>
    <ol class="pub-list">
      <li> ... </li>
    </ol>
    -->
  </main>
</div>

<script>
/* no nav tabs on this page; keep for future use if needed */
</script>


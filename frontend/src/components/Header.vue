<!-- RouterLinkをインポート -->
<script setup>
import { RouterLink } from 'vue-router'
</script>

<!-- HTML部分（Header部分） -->
<template>
  <header class="site-header">
    <div class="logo">
      <RouterLink to="/" class="logo-link">
        <img src="#" alt="logo" class="logo-image" />
        <span class="logo-text">Ayuka Tech Lab</span>
      </RouterLink>
    </div>
    <div class="sns">
      <a href="https://www.instagram.com/ayulab_post/" target="_blank" rel="noopener">
        <img src="@/assets/Instagram_logo.svg" alt="instagram" class="instagram-logo" />
      </a>
      <a href="https://x.com/ayulab_post" target="_blank" rel="noopener">
        <img src="@/assets/Xlogo.svg" alt="X" class="x-logo" />
      </a>
    </div>
    <nav class="nav-links">
      <RouterLink to="/about">ABOUT</RouterLink>
      <RouterLink to="/portfolio">PORTFOLIO</RouterLink>
      <RouterLink to="/blog">BLOG</RouterLink>
      <RouterLink to="/contact">CONTACT</RouterLink>
    </nav>
  </header>
</template>

<!-- CSS部分(Header部分) -->
<style scoped>
.site-header {
  display: flex;
  flex-direction: column;
  background-color: #ffffff;
  padding: 1rem 2rem;
  gap: 1rem;
}

.logo-link {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  text-decoration: none;
}

.logo-image {
  height: 40px;
}

.sns {
  display: flex;
  justify-content: flex-end;
  gap: 1rem;
  align-items: center;
}

.x-logo,
.instagram-logo {
  height: 20px;
}

.x-logo {
  background-color: #000000;
}

.logo-text {
  font-size: 1.5rem;
  font-weight: bold;
  font-family: 'Michroma', sans-serif;
  font-style: normal;
  color: rgb(0, 8, 255);
}

.nav-links {
  display: flex;
  gap: 1.5rem;
  justify-content: flex-end;
}

.nav-links a {
  text-decoration: none;
  color: #333;
  font-weight: 500;
  transition: color 0.3s;
}

.nav-links a:hover {
  color: #007bff;
}
</style>

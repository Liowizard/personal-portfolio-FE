<script setup lang="ts">
interface NavItem {
  label: string
  link: string
}

const navItems: NavItem[] = [
  { label: 'ABOUT', link: '#about' },
  { label: 'EXPERIENCE', link: '#experience' },
  { label: 'SKILLS', link: '#skills' },
  { label: 'EDUCATION', link: '#education' },
  { label: 'PROJECTS', link: '#projects' }
]
</script>

<template>
  <header class="header">
    <div class="logo">Ajesh</div>

    <nav class="nav-links">
      <ul>
        <li v-for="item in navItems" :key="item.label">
          <a :href="item.link">{{ item.label }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 1rem;
  color: #fff;
}

.logo {
  font-size: 2rem;
  font-weight: bold;
  color: #16f2b3;
}

ul {
  display: flex;
  gap: 1.5rem;
  list-style: none;
  margin: 0;
  padding: 0;
}

a {
  color: #ffffff;
  text-decoration: none;
  font-size: 0.9rem;
  font-weight: 500;
  transition: color 0.5s ease;
}

a:hover {
  color: #7e38f8; 
}

/* HIDE nav items on small screens */
@media (max-width: 768px) {
  .nav-links {
    display: none;
  }
}
</style>

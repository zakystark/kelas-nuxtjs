<!-- components/Header.vue -->
<template>
    <header class="header">
      <nav>
        <h1>MBKM</h1>
        <ul>
          <li><nuxt-link to="/">beranda</nuxt-link></li>
          <li><nuxt-link to="/about">daftar peserta</nuxt-link></li>
          <li><nuxt-link to="/contact">hasil nilai</nuxt-link></li>
        </ul>
      </nav>
    </header>
  </template>
  
  <script>
  export default {
    name: 'Header',
  }
  </script>
  
  <style scoped>
  .header {
    background-color: #333;
    color: white;
    padding: 1rem;
  }
  nav ul {
    list-style: none;
    display: flex;
    gap: 1rem;
  }
  </style>
  
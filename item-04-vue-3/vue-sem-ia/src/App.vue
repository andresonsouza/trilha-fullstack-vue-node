<script setup></script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  padding: 1rem 2rem;
  background-color: var(--primary-color);
}

nav ul {
  display: flex;
  gap: 1rem;
  list-style: none;
}

a {
  color: #FFFFFF;
  text-decoration: none;
}

nav ul li {
  color: #FFFFFF;
}

.router-link-active {
  color: #55efc4;
}

.logo a {
  color: #FFFFFF;
}

</style>

<template>
  <header>
    <div class="logo">
      <router-link to="/">TECH STORE</router-link>
    </div>
    <nav>
      <ul>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/produtos">Produtos</router-link></li>
        <li><router-link to="/contato">Contato</router-link></li>
      </ul>
    </nav>
  </header>
  <router-view />
</template>

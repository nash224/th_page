<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/item">Item</router-link> |
    <router-link to="/carousel">Carousel</router-link>
  </nav>
  <router-view/>
</template>

<script>

</script>


<style scoped>

nav {
  padding: 30px;
  /* justify-content: center; */
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
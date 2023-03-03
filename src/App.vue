<template>
  <!-- <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
    <router-link to="/register">Register</router-link>
    <router-link to="/contact">Contact</router-link>
    <router-link to="/products">Products</router-link>
  </nav> -->
  <NavBar/>
  <router-view/>
</template>

<script>
  import NavBar from '@/components/NavBar.vue'
  // import FooterVue from '@/components/FooterVue.vue'
  export default{
    name: 'App',
    components:{
      NavBar,
      // FooterVue
    }
  }
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>

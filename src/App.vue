<template>
  <Nav/>
  <router-view/>
  <Cards/>
  <Footer/>
</template>

<script>
import Nav from '@/components/NavBar.vue'
import Cards from '@/components/Cards.vue'
import Footer from '@/components/Footer.vue'

export default{
  components: {
    Nav,
    Cards,
    Footer
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

nav {
  padding: 30px;
  text-align: center;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>

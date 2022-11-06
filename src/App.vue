<template>
  <Navbar  :logo="logo_src" :alt="app_name" />
  <router-view/>
  <Footer />
</template>

<script>
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';

export default{
  components: {
    Navbar,
    Footer
  },
  data() {
    return {
      logo_src: "/img/logo.jpg",
      app_name: "Make your Shoes"
    }
  }
}

</script>

<style>
/* Toda a pagina vai seguir esse padrão */
* {
  font-family:Helvetica;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

/* Essa classe se repete em mais de uma pagina, por isso esta aqui */
.main-container{
  margin: 50px;
  min-height: 250px;
}

h1 {
text-align: center;
font-size: 42px;
margin-bottom:30px;
color: #222;
}
</style>

<template>
  <div id="nav">
    <router-link to="/" id="logo-url">
        <img :src="logo" :alt="alt" id="logo">
    </router-link>
    <router-link to="/">Home</router-link> 
    <router-link to="/pedidos">Pedidos</router-link>
  </div>
</template>

<script>
export default {
    name: "Navbar",
    props: [ "logo", "alt"]
}
</script>

<style scoped>

/* Navbar com os elementos a direita da tela */
#nav {
  background-color: #222;
  border-bottom: 4px solid #111;
  padding: 15px 50px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

/* Logo vai para esquerda 
mas não interfere no id nav*/
#nav #logo-url{
  margin: auto;
  margin-left: 0;
}

/* tamnaho do logo */
#logo {
  width: 40px;
  height: 40px;
}

/* maniplacao da cor do texto */
#nav a{
  color: #FCBA03;
  text-decoration: none;
  margin: 12px;
  transition: .05s;
}
#nav a:hover{
  color: #FFF;
}

</style>
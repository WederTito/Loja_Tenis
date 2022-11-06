<template>
  <footer id="footer">
    <p>Personalize seu tenis &copy; 2022</p>
  </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style scoped>

/* Configurações do footer para que ele fique alinhado ao centro */
#footer{
    height: 200px;
    background-color: #222;
    border-top: 4px solid #111;
    color: #FCBA03;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
  }
</style>
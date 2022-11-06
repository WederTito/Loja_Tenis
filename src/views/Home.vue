<template>
  <Banner />
  <div class="main-container">
    <h1>Monte Seu tenis</h1>
    <br>
    <ShoesForm />
 </div>
</template>

<script>
import Banner from '../components/Banner.vue';
import ShoesForm from '../components/ShoesForm.vue';

export default {
  name: "Home",
  components: {
    Banner,
    ShoesForm
  }
}

</script>

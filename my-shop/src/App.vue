<template>
  <img alt="Vue logo" src="./assets/logo.png">
<Productcard
name="Українська вишиванка"
description="Стильна вишиванка з традиційним орнаментами"
price="1500"
image="https://encrypted-tbn0.gstatic.com/images?q=tbn:
ANd9GcSCrKn_Ds5Odt9WJTjZWh47MBe6HY6WowLDwCIG140a3w&s=10"




/>
</template>

<script>
import productcard from './components/productcard.vue';



export default {
  name: 'App',
  components: {
    productcard
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

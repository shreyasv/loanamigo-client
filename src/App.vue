<template>
  <div id="base">

    <img src="./assets/logo.png">

    <router-view/>

    <Footer/>
  </div>
</template>


<script>

import Footer from '@/components/Footer.vue'
export default { // Question: why do I need to export this?

  components: {
    Footer
  }
}

</script>

<style>
#base {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

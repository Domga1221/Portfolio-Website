<template>
  <div id="Home">
    <div class="text-center py-4 bg-secondary text-light">
        <b-img thumbnail fluid src="http://cdn.dota2.com/apps/dota2/images/heroes/mars_full.png?" alt="Image 1"></b-img>
        <h1 class="mt-2">Dominik</h1>
        <h3>Computer Science Student</h3>
        <b-button href="https://github.com/Domga1221" target="_blank" class="btn btn-light btn-lg btn-outline-dark">GitHub</b-button>
    </div>
    <Home-Projects></Home-Projects>
  </div>
</template>

<script>
import HomeProjects from '../Home/HomeProjects.vue'
export default {
    components:{
        'Home-Projects': HomeProjects,
    },

    data (){
      return {
        imgSrc: require('../../assets/Bild.png')
      }
    }
}
</script>

<style scoped>
  
</style>
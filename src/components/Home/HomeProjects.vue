<template>
  <div id="HomeProjects" class="text-center bg-light">
    
    <section class="protfolio py-4">

      <h1 class="">Projects</h1>
      <p>These are a sample of my Projects</p>

      <div class="container">
        <div class="row">
          <div class="col-md-4">

            <HomeProjectCard v-bind:description="data.description1"
            v-bind:imgSrc="data.imgSrc1"
            v-bind:title="data.title1"
            v-bind:url="data.url1">
            </HomeProjectCard>

            <br />
          </div>
          <div class="col-md-4">
            
            <HomeProjectCard v-bind:description="data.description2"
            v-bind:imgSrc="data.imgSrc2"
            v-bind:title="data.title2"
            v-bind:url="data.url2">
            </HomeProjectCard>

            <br />
          </div>
          <div class="col-md-4">

            <HomeProjectCard v-bind:description="data.description3"
            v-bind:imgSrc="data.imgSrc3"
            v-bind:title="data.title3"
            v-bind:url="data.url3">
            </HomeProjectCard>

          </div>
        </div>
      </div>

    </section>


  </div>
</template>


<script>
import HomeProjectCard from './HomeProjectCard.vue'
import data from '../../mixins/data.js'

export default {
  data() {
    return {
      data: data,

      
    }
  },

  components: {
    HomeProjectCard
  }
};
</script>


<style scoped>
.protfolio {
  background-color: #34345238;
}
</style>
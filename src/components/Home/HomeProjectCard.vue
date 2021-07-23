<template>
  <div id="HomeProjectCard" class="card">
    <div class="card-head">
      <img
        class="img-custome mt-4"
        v-bind:src="imgSrc"/>
      <h2 class="mt-2">{{title}}</h2>
    </div>
    <hr />
    <div class="card-body">
      <p class="text-justify">{{description}}</p>
      <b-button v-bind:href="url" target="_blank" class="">More</b-button>
    </div>
  </div>
</template>


<script>

export default {
    data() {
        return {
          
        }
    },

    props: {
        description: {},
        title: {},
        imgSrc: {},
        url: {}
    }
};
</script>


<style scoped>
.img-custome {
  width: 135px;
  height: 240px;
}
</style>
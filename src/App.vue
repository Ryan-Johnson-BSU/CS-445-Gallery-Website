<script setup>
import HelloWorld from './components/HelloWorld.vue'
var images = ["pexels-asphotograpy-101808.jpg", "pexels-brettjordan-842528.jpg", "pexels-eye4dtail-114741.jpg",
  "pexels-eye4dtail-333837.jpg", "pexels-eye4dtail-333838.jpg", "pexels-ingo-14721.jpg", "pexels-kaboompics-5930.jpg",
  "pexels-marcin-szmigiel-14638-67094.jpg", "pexels-nietjuhart-612800.jpg", "pexels-revac-film-s-photography-10400-109361.jpg"
]



</script>



<template>
  <div>
    <HelloWorld msg="Gallery of Key Photos" />
    
    <div v-for = "image in images"  >
        
        <img v-bind:src="image" height="500" width="750">
      </div>
   
  </div>

</template>

<style scoped>
.logo {
  height: 12em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>

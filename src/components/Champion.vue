<template>
  <div class="champion">
    <a class="img-link" href=""><img :src='getImgUrl(champion.id)' v-bind:alt='champion.name'/></a>
    <h2 style="font-size:5vw;">{{champion.name}} | {{champion.role}} <img class="role" src="../assets/toplane.png"/> </h2>
    <p></p>
  </div>
</template>

<script>
export default { 
  name: 'Champion',
  props: {
    champion: Object
  },
  methods: {
    getImgUrl(id){
      var images = require.context('../assets/', false, /\.jpg$/)
      return images('./' + id + ".jpg")
    }
  }
}
</script>

<style scoped>

@font-face {
    font-family: "Friz Quadrata";
    src: url('../fonts/Friz.ttf');
}

.role{
  width: 10%;
}

.img-link img{
  width: 100%;
}

img:hover{
 
  cursor: pointer;
}

h2{
  font-family: "Friz Quadrata";
  margin-top: -80px;
  color: white;
  text-align: left;
  padding-left: 40px;

}

@media screen and (min-width: 800px) {
  h2{
  
  margin-top: -200px;
  

}
} 



</style>
<template>
  <div class="fondo">
    <div  v-for="(things,index) in characters" :key="index">
      <img :src="things.image">
      <h2>{{things.name}}</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: 'InfoPersonajes',
  props: {
    characters:{
      type: Array,
      require: true
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
template{
  margin: 0;
}
.fondo{
  background-image: url('https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png');
  background-size: cover;
  background-position: center;
}
img{
  border-radius: 50%;
  margin-top: 2em;
  margin-left: 2em;
  margin-right: 2em;
  height: 10em;
}
h2{
  color: green;
  font-size: 2em;
  font-weight: bold;
  display: inline;
}
</style>

<template>
  <div>
    <div class="fondo" v-for="(things,index) in characters" :key="index">
      <img :src="things.image"><span>{{things.name}}</span>
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
.fondo{
  background-image: url('https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png');
  background-size: cover;
  background-position: center;
  margin: 0;
}
img{
  border-radius: 50%;
  margin-top: 2em;
  margin-left: 2em;
  margin-right: 2em;
  height: 5em;
}
span{
  color: green;
  font-size: 2em;
  font-weight: bold;
}
</style>

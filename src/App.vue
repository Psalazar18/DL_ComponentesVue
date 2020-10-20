<template>
  <div id="app">
    <InfoPersonajes :characters="DataPersonajes"/>
  </div>
</template>

<script>
import InfoPersonajes from './components/InfoPersonajes.vue'

export default {
  name: 'App',
  data() {
    return {
      DataPersonajes: [
        {name: 'Rick Sanchez', image: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg'},
        {name: 'Morty Smith', image: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg'},
        {name: 'Summer Smith', image: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg'},
        {name: 'Beth Smith', image: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg'},
        {name: 'Jerry Smith', image: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg'}
      ]
      
    } 
    
  },
  components: {
    InfoPersonajes
  }
}
</script>

<style>

</style>

<template>
  <div>
    <h1>Desafío</h1>
    <Avatar
      v-for="(personaje, $index) of personajes"
      :key="$index"
      :nombre="personaje.nombre"
      :imagen="personaje.src"
    /> 
  </div>
</template>

<script>
import Avatar from "@/components/Avatar.vue";
export default {
  name: "App",
  components: { 
    Avatar 
  },
  data: () => ({
    personajes: [
      {
        nombre: "Rick Sanchez",
        src: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
      },
      {
        nombre: "Morty Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
      },
      {
        nombre: "Summer Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
      },
      {
        nombre: "Beth Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
      },
      {
        nombre: "Jerry Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
      },
    ]
  })
}
</script>

<style>

body {
  font-family: 'Creepster', cursive;
  background-image: url("../src/assets/background.png");
  background-size: cover;
  padding-bottom: 9rem;
}
</style>

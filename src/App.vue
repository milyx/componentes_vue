<template>
  <div id="app">
    <FigurAnimada
      v-for="(personaje, i) in personajes"
      :key="i"
      :lolito="personaje"
    />
  </div>
</template>

<script>
import FigurAnimada from "@/components/FigurAnimada.vue";
export default {
  name: "App",
  components: {
    FigurAnimada,
  },
  data() {
    return {
      personajes: [
        {
          name: "Morty Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
        },
        {
          name: "Morty Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
        },
        {
          name: "Summer Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
        },
        {
          name: "Beth Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
        },
        {
          name: "Beth Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
        },
        {
          name: "Jerry Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/6.jpeg",
        },
      ],
    };
  },
  img() {
    return {
      fondo: [
        {
          src: "https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png",
        },
      ],
    };
  },

  props: {
    text: String,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #097737;

  padding: 30px 50px;
  background-image: url(https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png);
}
</style>

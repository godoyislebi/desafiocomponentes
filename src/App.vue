<template>
  <div id="app">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <ListaRick
            v-for="(datoRick, i) in datosRick"
            :key="i"
            :datos="datoRick"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ListaRick from "@/components/ListaRick.vue";

export default {
  name: "App",
  components: {
    ListaRick,
  },
  data() {
    return {
      datosRick: [
        {
          name: "Rick Sanchez",
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
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-image: url("https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.img-circle {
  border-radius: 50%;
  width: 15%;
  height: auto;
  margin-right: 2%;
}
.tipograph-rick {
  font-family: "Bangers", cursive;
  color: #62a838;
  text-shadow: 2px -2px 1px #000;
}
.bg-none {
  background-color: transparent;
}
</style>

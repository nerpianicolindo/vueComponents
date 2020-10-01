<template>
  <div id="app">
    <boton
      v-for="boton in botones"
      :color="boton.color"
      :enlace="boton.enlace"
      :anchor="boton.anchor"
    />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import Gato from "./components/Gato";
import Boton from "./components/Boton";
export default {
  name: "App",
  components: {
    HelloWorld,
    Gato,
    Boton,
  },
  data() {
    return {
      botones: [
        { enlace: "http://google.es", anchor: "Wmedia", color: "red" },
        { enlace: "http://google.es", anchor: "Wmedia", color: "blue" },
        { enlace: "http://google.es", anchor: "Wmedia", color: "yellow" },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

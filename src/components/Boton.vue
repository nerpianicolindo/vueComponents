<template>
  <a class="boton" :sytle="'background-color: ' + color" :href="enlace">
    <Destino></Destino>
  </a>
</template>

<script>
import Destino from "@/components/Destino.vue";

export default {
  //props: ["color", "enlace", "anchor"],
  props: {
    color: String,
    enlace: {
      type: String,
      default: "https://www.google.es",
    },
    anchor: String,
  },
  components: {
    Destino,
  },
};
</script>

<style>
</style>
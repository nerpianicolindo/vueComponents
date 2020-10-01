<template>
  <img :src="urlCompleta" />
</template>

<script>
export default {
  name: "Gato",
  props: {
    msg: String,
  },
  data() {
    return {
      ancho: Math.floor(Math.random() * 600) + 100,
      alto: Math.floor(Math.random() * 600) + 100,
    };
  },
  computed: {
    urlCompleta() {
      return `https://placekitten.com/${this.ancho}/${this.alto}`;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

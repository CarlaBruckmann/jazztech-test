<template>
  <Card />
</template>

<script>
import Card from "./components/Card.vue";

export default {
  name: "App",
  components: {
    Card,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Exo:wght@500&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Ubuntu&display=swap");
:root {
  --white: #ffffff;
  --black: #000004;
  --blue-accent: #b1d0d6;
  --blue-dark: #092052;
  --font-primary: "Exo";
  --font-secondary: "Ubuntu";
}
</style>

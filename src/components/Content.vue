<template>
  <section>
    <Title />
    <Accordion />
  </section>
</template>

<script>
import Title from "./Title.vue";
import Accordion from "./Accordion.vue";

export default {
  name: "Content",
  components: {
    Title,
    Accordion,
  },
};
</script>

<style scoped>
section {
  background-color: var(--blue-dark);
  height: 100%;
  flex: 1 1 600px;
}
div {
  margin: 20px;
}
</style>
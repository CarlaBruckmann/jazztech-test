<template>
  <section>
    <Title />
  </section>
</template>

<script>
import Title from "./Title.vue";
export default {
  name: "Content",
  components: {
    Title,
  },
};
</script>

<style scoped>
section{
  background-color: var(--blue-dark);
  height: 100%;
  flex: 1 1 600px; 
}
div {
  margin: 20px;
}

</style>
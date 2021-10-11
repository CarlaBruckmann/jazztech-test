<template>
  <div class="card">
    <Header />
    <Content />
  </div>
</template>

<script>
import Content from "./Content.vue";
import Header from "./Header.vue";

export default {
  name: "Card",
  components: {
    Content,
    Header,
  },
};
</script>

<style>
.card {
  width: 80vw;
  max-width: 1300px;
  height: auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  margin: 10px auto;
  background-color: var(--black);
}
</style>

<template>
  <div class="card">
    <WrapperHeader />
    <Content/>
  </div>
</template>

<script>
import Content from "./Content.vue";
import WrapperHeader from "./Header.vue";

export default {
  name: "Card",
  components: {
    Content,
    WrapperHeader,
  },
};
</script>

<style>
.card {
  width: 80vw;
  max-width: 1300px;
  height: 600px;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  margin: 10px auto;
}

</style>

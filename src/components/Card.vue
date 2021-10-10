<template>
  <div class="card">
    <WrapperHeader />
    <Wrapper />
  </div>
</template>

<script>
import Wrapper from "./Wrapper.vue";
import WrapperHeader from "./WrapperHeader.vue";

export default {
  name: "Card",
  components: {
    Wrapper,
    WrapperHeader,
  },
};
</script>

<style>
.card {
  width: 80vw;
  max-width: 1535px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  margin: 30px auto;
}
</style>

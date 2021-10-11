<template>
  <section>
    <User />
    <Button />
  </section>
</template>

<script>
import Button from "./Button.vue";
import User from "./User.vue";
export default {
  name: "Header",
  components: {
    Button,
    User,
  },
};
</script>

<style scoped>
section {
  background: url("./assets/logo.png") no-repeat;
  background-size: 120%;
  background-position: center;
  background-color: var(--black);
  height: 610px;
  display: flex;
  flex: 1 1 300px;
  justify-content: space-between;
  align-items: flex-end;
}
div {
  margin: 30px 20px;
}
button {
  margin: 30px 30px 50px 30px;
}

@media screen and (max-width: 1124px) {
  section {
    height: 200px;
    background-position: center top;
    background-size: 70%;
  }
}

@media screen and (max-width: 670px) {
  section {
    background-position: center top;
    background-size: 100%;
  }
}
</style>
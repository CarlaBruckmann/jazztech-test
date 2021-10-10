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
  name: "WrapperHeader",
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
  width: 50%;
  height: 600px;
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
}
div{
  padding: 30px;
}
button{
    margin: 30px 30px 40px 30px;
}
</style>
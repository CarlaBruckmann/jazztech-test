<template>
  <div>
    <img src="./assets/user.png" alt="User image" />
    <p>Madelyn<br />Stillwell</p>
  </div>
</template>

<script>
export default {
  name: "User",
};
</script>

<style scoped>
div {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
}
p {
  color: var(--white);
  font-family: var(--font-secundary);
  font-size: 12px;
  text-align: center;
  margin-left: 10px;
  cursor:default;
}
img {
  margin: 10px;
  cursor: pointer;
}
</style>
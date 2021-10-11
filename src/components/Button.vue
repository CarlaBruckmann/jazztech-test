<template>
  <button role="button" aria-label="logout">Logout</button>
</template>

<script>
export default {
  name: "Button",
};
</script>

<style scoped>
button {
  text-decoration: uppercase;
  padding: 5px 10px;
  border: solid 1px var(--blue-accent);
  background: var(--blue-dark);
  font-family: var(--font-primary);
  color: var(--white);
  text-transform: uppercase;
  cursor: pointer;
}
button:hover,
button:focus {
  transform: scale(1.05);
  transition: 0.2s ease all;
}
</style>
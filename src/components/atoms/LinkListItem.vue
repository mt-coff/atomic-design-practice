<template>
  <router-link :to="to" replace><slot /></router-link>
</template>

<script>
export default {
  name: "link-list-item",
  props: {
    to: {
      type: String,
      required: true
    }
  }
};
</script>

<style scoped>
a {
  font-weight: bold;
  color: #2c3e50;
}
a.router-link-exact-active {
  color: #42b983;
}
</style>

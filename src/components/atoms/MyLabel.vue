<template>
  <label><slot /></label>
</template>

<script>
export default {
  name: "my-label"
};
</script>

<style scoped>
label {
  font-weight: bold;
}
</style>

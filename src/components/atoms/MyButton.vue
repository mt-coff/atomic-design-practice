<template>
  <button class="button" @click="onClick"><slot></slot></button>
</template>

<script>
export default {
  name: "my-button",

  methods: {
    onClick() {
      this.$emit("click");
    }
  }
};
</script>

<style scoped>
button {
  border: 1px solid #252525;
  border-radius: 8px;
  background-color: #ffffff;
  cursor: pointer;
  font-size: 15px;
  padding: 3px 10px;
}
</style>

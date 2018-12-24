<template>
  <input
    @input="onInput"
    :value="value"
    :type="type"
    :placeholder="placeholder"
  />
</template>

<script>
export default {
  name: "my-input",
  props: {
    value: {
      type: String,
      default: ""
    },
    type: {
      type: String,
      default: "text"
    },
    placeholder: {
      type: String
    }
  },
  methods: {
    onInput(event) {
      this.$emit("input", event.target.value);
    }
  }
};
</script>

<style scoped>
input {
  border: 1px solid #252525;
  border-radius: 8px;
  background-color: #ffffff;
  font-size: 15px;
  padding: 3px 5px;
}
</style>

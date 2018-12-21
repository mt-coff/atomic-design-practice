<template>
  <textarea
    @input="onInput"
    :value="value"
    :rows="rows"
    :placeholder="placeholder"
  />
</template>

<script>
export default {
  name: "my-text-area",
  props: {
    value: {
      type: String,
      default: ""
    },
    rows: {
      type: Number,
      default: 2
    },
    placeholder: {
      type: String
    }
  },
  methods: {
    onInput(newValue) {
      this.$emit("input", newValue);
    }
  }
};
</script>

<style scoped>
textarea {
  border: 1px solid #252525;
  border-radius: 8px;
  background-color: #ffffff;
  font-size: 15px;
  padding: 3px 5px;
  min-width: 500px;
}
</style>

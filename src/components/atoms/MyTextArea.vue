<template>
  <textarea
    :value="value"
    :rows="rows"
    :placeholder="placeholder"
    @input="onInput"
  />
</template>

<script>
export default {
  name: "my-text-area",
  props: {
    value: {
      type: String
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
    onInput(event) {
      this.$emit("input", event.target.value);
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

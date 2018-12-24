<template>
  <img :src="src" :alt="alt" />
</template>

<script>
export default {
  name: "my-image",
  props: {
    src: {
      type: String,
      required: true
    },
    alt: {
      type: String
    }
  }
};
</script>

<style scoped></style>

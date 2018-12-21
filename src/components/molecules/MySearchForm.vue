<template>
  <div>
    <my-input type="text" placeholder="Search" />
    <my-button>Search</my-button>
  </div>
</template>

<script>
import MyButton from "@/components/atoms/MyButton.vue";
import MyInput from "@/components/atoms/MyInput.vue";

export default {
  name: "my-search-form",
  components: {
    MyButton,
    MyInput
  }
};
</script>

<style scoped></style>

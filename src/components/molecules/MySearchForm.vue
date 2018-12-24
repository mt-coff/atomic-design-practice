<template>
  <div>
    <my-label>Search This Site</my-label>
    <div>
      <my-input class="search-input" type="text" placeholder="Search" />
      <my-button>Search</my-button>
    </div>
  </div>
</template>

<script>
import MyLabel from "@/components/Atoms/MyLabel.vue";
import MyButton from "@/components/Atoms/MyButton.vue";
import MyInput from "@/components/Atoms/MyInput.vue";

export default {
  name: "my-search-form",
  components: {
    MyLabel,
    MyButton,
    MyInput
  }
};
</script>

<style scoped>
.search-input {
  margin-right: 1rem;
}
</style>

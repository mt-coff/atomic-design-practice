<template>
  <header>
    <my-title>Practice</my-title>
    <search-form class="search-form" />
  </header>
</template>

<script>
import MyTitle from "@/components/Atoms/MyTitle.vue";
import SearchForm from "@/components/Molecules/MySearchForm.vue";

export default {
  name: "my-header",
  components: {
    MyTitle,
    SearchForm
  }
};
</script>

<style scoped>
header {
  background-color: #24292e;
  display: flex;
  justify-content: space-between;
  padding: 0 1rem;
  color: #ffffff;
}
.search-form {
  margin: auto 0;
}
</style>

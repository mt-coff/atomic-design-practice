<template>
  <div class="home">
    <my-feed-form />
    <my-search-form />
  </div>
</template>

<script>
import MyFeedForm from "@/components/molecules/MyFeedForm.vue";
import MySearchForm from "@/components/molecules/MySearchForm.vue";

export default {
  name: "home",
  components: {
    MyFeedForm,
    MySearchForm
  }
};
</script>

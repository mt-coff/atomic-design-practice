<template>
  <div class="page3">
    <my-title>Page3</my-title>
    <my-article>
      page3page3page3page3page3page3page3page3page3page3page3page3.
      page3page3page3page3page3page3page3page3page3page3page3page3page3page3.
      page3page3page3page3page3page3page3page3page3page3page3page3page3page3page3page3page3page3page3page3page3page3page3page3.
      page3page3page3page3page3page3page3page3page3page3page3page3
      page3page3page3page3page3page3page3page3page3page3page3page3
    </my-article>
  </div>
</template>

<script>
import MyTitle from "@/components/Atoms/MyTitle.vue";
import MyArticle from "@/components/Organisms/MyArticle.vue";

export default {
  name: "page3",
  components: {
    MyTitle,
    MyArticle
  }
};
</script>

<style scoped>
.page3 {
  padding: 1rem 2rem;
}
</style>

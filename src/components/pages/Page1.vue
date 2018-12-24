<template>
  <div class="page1">
    <my-title>Page1</my-title>
    <my-article>
      page1page1page1page1page1page1page1page1page1page1page1page1.
      page1page1page1page1page1page1page1page1page1page1page1page1page1page1.
      page1page1page1page1page1page1page1page1page1page1page1page1page1page1page1page1page1page1page1page1page1page1page1page1.
      page1page1page1page1page1page1page1page1page1page1page1page1
      page1page1page1page1page1page1page1page1page1page1page1page1
    </my-article>
  </div>
</template>

<script>
import MyTitle from "@/components/Atoms/MyTitle.vue";
import MyArticle from "@/components/Organisms/MyArticle.vue";

export default {
  name: "page1",
  components: {
    MyTitle,
    MyArticle
  }
};
</script>

<style scoped>
.page1 {
  padding: 1rem 2rem;
}
</style>

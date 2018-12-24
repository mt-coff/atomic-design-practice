<template>
  <div class="page2">
    <my-title>Page2</my-title>
    <my-article>
      page2page2page2page2page2page2page2page2page2page2page2page2.
      page2page2page2page2page2page2page2page2page2page2page2page2page2page2.
      page2page2page2page2page2page2page2page2page2page2page2page2page2page2page2page2page2page2page2page2page2page2page2page2.
      page2page2page2page2page2page2page2page2page2page2page2page2
      page2page2page2page2page2page2page2page2page2page2page2page2
    </my-article>
  </div>
</template>

<script>
import MyTitle from "@/components/Atoms/MyTitle.vue";
import MyArticle from "@/components/Organisms/MyArticle.vue";

export default {
  name: "page2",
  components: {
    MyTitle,
    MyArticle
  }
};
</script>

<style scoped>
.page2 {
  padding: 1rem 2rem;
}
</style>

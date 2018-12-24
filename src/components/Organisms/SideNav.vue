<template>
  <nav>
    <my-title>Menu</my-title>
    <link-list :link-list="linkList" />
  </nav>
</template>

<script>
import MyTitle from "@/components/Atoms/MyTitle.vue";
import LinkList from "@/components/Molecules/LinkList.vue";

export default {
  name: "side-nav",
  components: {
    MyTitle,
    LinkList
  },
  data() {
    return {
      linkList: { home: "/", page1: "page1", page2: "page2", page3: "page3" }
    };
  }
};
</script>

<style scoped>
nav {
  border-right: solid 1px #dddddd;
  padding: 0 1.5rem;
}
</style>

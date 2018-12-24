<template>
  <ul>
    <li v-for="(link, key) in linkList" :key="key">
      <link-list-item :to="link">{{ key }}</link-list-item>
    </li>
  </ul>
</template>

<script>
import LinkListItem from "@/components/Atoms/LinkListItem.vue";

export default {
  name: "link-list",
  components: {
    LinkListItem
  },
  props: {
    linkList: {
      type: Object,
      required: true
    }
  }
};
</script>

<style scoped></style>

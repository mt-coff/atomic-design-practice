<template>
  <div class="container">
    <my-image :src="src" :alt="alt" />
    <paragraph><slot /></paragraph>
  </div>
</template>

<script>
import Paragraph from "@/components/Atoms/Paragraph.vue";
import MyImage from "@/components/Atoms/MyImage.vue";

export default {
  name: "paragraph-with-image",
  components: {
    Paragraph,
    MyImage
  },
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

<style scoped>
.container {
  display: inline-block;
}
</style>

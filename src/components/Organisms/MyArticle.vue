<template>
  <div>
    <paragraph-with-image src="https://placehold.jp/400x400.png">
      <slot />
    </paragraph-with-image>
    <feed-form v-model="value" @onClear="onClear" @onSubmit="onSubmit" />
  </div>
</template>

<script>
import ParagraphWithImage from "@/components/Molecules/ParagraphWithImage.vue";
import FeedForm from "@/components/Molecules/FeedForm.vue";

export default {
  name: "my-article",
  components: {
    ParagraphWithImage,
    FeedForm
  },
  data() {
    return {
      value: ""
    };
  },
  methods: {
    onClear() {
      this.value = "";
    },
    onSubmit() {
      confirm("Summitted!");
    }
  }
};
</script>

<style scoped></style>

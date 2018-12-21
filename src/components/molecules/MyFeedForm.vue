<template>
  <div>
    <my-text-area placeholder="Please input your feed!" :rows="5" />
    <div>
      <my-button>clear</my-button>
      <my-button>submit</my-button>
    </div>
  </div>
</template>

<script>
import MyButton from "@/components/atoms/MyButton.vue";
import MyTextArea from "@/components/atoms/MyTextArea.vue";

export default {
  name: "my-feed-form",
  components: {
    MyButton,
    MyTextArea
  }
};
</script>

<style scoped></style>

<template>
  <div class="home">
    <my-title>Home</my-title>
    <paragraph>
      homehomehomehomehomehomehomehomehomehomehomehomehomehome
      homehomehomehomehomehomehomehomehomehomehomehomehomehome
      homehomehomehomehomehomehomehomehomehomehomehomehomehome
      homehomehomehomehomehomehomehomehomehomehomehomehomehome
      homehomehomehomehomehomehomehomehomehomehomehomehomehome
      homehomehomehomehomehomehomehomehomehomehomehomehomehome
      homehomehomehomehomehomehomehomehomehomehomehomehomehome
      homehomehomehomehomehomehomehomehomehomehomehomehomehome
    </paragraph>
  </div>
</template>

<script>
import MyTitle from "@/components/Atoms/MyTitle";
import Paragraph from "@/components/Atoms/Paragraph";

export default {
  name: "home",
  components: {
    MyTitle,
    Paragraph
  }
};
</script>

<style scoped>
.home {
  padding: 1rem 2rem;
}
</style>

<template>
  <div class="container">
    <my-text-area
      :value="value"
      @input="onInput"
      :rows="5"
      placeholder="Please input your feed!"
    />
    <div class="is-right">
      <my-button class="dainger" @click="onClear">clear</my-button>
      <my-button class="submit" @click="onSubmit">submit</my-button>
    </div>
  </div>
</template>

<script>
import MyButton from "@/components/Atoms/MyButton.vue";
import MyTextArea from "@/components/Atoms/MyTextArea.vue";

export default {
  name: "feed-form",
  components: {
    MyButton,
    MyTextArea
  },
  props: {
    value: {
      type: String
    }
  },
  methods: {
    onInput(newValue) {
      this.$emit("input", newValue);
    },
    onClear() {
      this.$emit("onClear");
    },
    onSubmit() {
      this.$emit("onSubmit");
    }
  }
};
</script>

<style scoped>
.container {
  display: inline-block;
}
.is-right {
  text-align: right;
}
.dainger {
  background-color: #ff0000;
  color: #ffffff;
  font-weight: bold;
}
.submit {
  background-color: #42b983;
  color: #ffffff;
  font-weight: bold;
}
</style>

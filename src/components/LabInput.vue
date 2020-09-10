<script>
export default {
  computed: {
    inputEvents() {
      return {
        mouseenter: this.showTooltip,
        input: this.updateForm
      };
    }
  },
  methods: {
    showTooltip() {
      console.log("Tooltip");
    },
    updateForm() {
      console.log("Update");
    },
    testProps(item) {
      if (item === "article") {
        return {
          attrs: {
            test: "hello"
          }
        };
      } else {
        return {
          attrs: {
            test: "world"
          }
        };
      }
    }
  }
};
</script>

<template>
  <input type="text" v-on="inputEvents" v-bind="testProps('article').attrs" />
</template>

<style></style>

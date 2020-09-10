<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <MultipleElements />
  </div>
</template>

<script>
// @ is an alias to /src
import MultipleElements from "@/components/MultipleElements.vue";

export default {
  name: "Home",
  components: {
    MultipleElements
  }
};
</script>

<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <RenderExample>
      <h1>Render Title</h1>
    </RenderExample>
  </div>
</template>

<script>
// @ is an alias to /src
import RenderExample from "@/components/RenderExample.vue";

export default {
  name: "Home",
  components: {
    RenderExample
  }
};
</script>

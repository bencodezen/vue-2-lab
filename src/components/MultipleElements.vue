<script>
export default {
  data() {
    return {
      cmsData: [
        `<h1>My Blog Title</h1>`,
        `<h2>Introduction</h2>`,
        `<p>This is my <strong>topic</strong>!</p>`
      ]
    };
  },
  computed: {
    blogPost() {
      return this.cmsData.join("");
    }
  }
};
</script>

<template>
  <article>
    <h1>Multiple Elements From CMS</h1>
    <h2>Rendering HTML Directly</h2>
    <div v-html="cmsData"></div>
    <h2>Use Computed Value</h2>
    <div v-html="blogPost"></div>
  </article>
</template>

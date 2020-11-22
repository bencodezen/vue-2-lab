<script>
export default {
  render(createElement) {
    return createElement(
      "div",
      { class: { button: true } },
      this.$slots.default
    );
  }
};
</script>

<style></style>

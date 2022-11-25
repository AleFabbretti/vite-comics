<script>
import AppSection from "./AppSection.vue";

export default {
  name: "AppMain",
  components: {
    AppSection,
  },
};
</script>

<template>
  <main>
    <section class="jumbotron">
      <img src="../assets/jumbotron.jpg" alt="" />
    </section>
    <AppSection />
  </main>
</template>

<style lang="scss" scoped>
main {
  background-color: var(--secondary-color);
  & .jumbotron img {
    width: 100%;
    max-height: 400px;
    object-fit: cover;
    object-position: top;
  }
}
</style>

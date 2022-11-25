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
    <div class="container">
      <p>--> Content goes here</p>
    </div>
  </main>
</template>

<style lang="scss" scoped>
main {
  background-color: var(--secondary-color);
  height: 130px;
  color: white;
  padding: 50px 0;
  font-size: 23px;
}
</style>

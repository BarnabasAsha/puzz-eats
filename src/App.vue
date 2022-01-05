<template>
  <div>
    <Header />
    <main>
      <Hero />
      <SectionOne />
    </main>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Hero from "./components/Hero.vue";
import SectionOne from "./components/SectionOne.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
    SectionOne,
  },
};
</script>

<style lang="scss" src="./styles/app.scss"></style>

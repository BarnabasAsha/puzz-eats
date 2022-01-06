<template>
  <div>
    <Header />
    <main>
      <Hero />
      <SectionOne />
      <MealPlans />
      <Recipes />
      <Opinions />
      <Options />
      <Extras />
      <Community />
      <Footer />
    </main>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Hero from "./components/Hero.vue";
import SectionOne from "./components/SectionOne.vue";
import MealPlans from "./components/MealPlans/MealPlans.vue";
import Recipes from "./components/Recipes/Recipes.vue";
import Opinions from "./components/Opinions.vue";
import Options from "./components/Options/Options.vue";
import Extras from "./components/Extras.vue";
import Community from "./components/Community.vue";
import Footer from "./components/Footer/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
    SectionOne,
    MealPlans,
    Recipes,
    Opinions,
    Options,
    Extras,
    Community,
    Footer,
  },
};
</script>

<style lang="scss" src="./styles/app.scss"></style>

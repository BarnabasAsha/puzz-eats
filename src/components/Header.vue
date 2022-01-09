<template>
  <header>
    <div class="container">
      <div class="header">
        <div class="logo">
          <img src="../assets/puzz-eats.png" alt="Puzz eats" />
        </div>
        <nav class="header_nav">
          <ul>
            <li>
              <a href="#">Recipes</a>
            </li>
            <li>
              <a href="#">Meal Plans</a>
            </li>
            <li>
              <a href="#">Shop</a>
            </li>
            <li>
              <a href="#">Combo Pack</a>
            </li>
          </ul>
          <button class="cta"><a href="#">Create Meal Plan</a></button>
        </nav>
        <button
          @click="() => (status = !status)"
          class="header_menu"
          :class="status ? 'active' : ''"
        >
          <span></span>
          <span></span>
          <span></span>
        </button>
      </div>
    </div>
  </header>
  <MobileNav v-if="status" />
</template>

<script>
import MobileNav from "./MobileNav.vue";
import { ref } from "vue";

export default {
  name: "Header",
  components: {
    MobileNav,
  },
  setup() {
    const status = ref(false);
    return { status };
  },
};
</script>

<style lang="scss" src="../styles/header.scss"></style>

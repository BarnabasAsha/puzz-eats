<template>
  <div class="container">
    <div class="options">
      <div class="_left">
        <div class="subtitle">Flavor Explorer</div>
        <h2>
          Explore Inclusive <br />
          Diet Options.
        </h2>
      </div>
      <div class="_right">
        <button class="cta"><a href="#">Request An Option</a></button>
      </div>
    </div>
    <div class="options_flow">
      <Option
        v-for="option in options"
        :key="option.title"
        :img="option.img"
        :title="option.title"
      />
    </div>
  </div>
</template>

<script>
import Option from "./Option.vue";
import { ref } from "vue";

export default {
  name: "Options",
  components: {
    Option,
  },
  setup() {
    const options = ref([
      {
        title: "vegan",
        img: "vegan",
      },
      {
        title: "low carb",
        img: "low-carb",
      },
      {
        title: "gluten-free",
        img: "gluten-free",
      },
    ]);
    return { options };
  },
};
</script>

<style lang="scss" src="../../styles/options.scss"></style>

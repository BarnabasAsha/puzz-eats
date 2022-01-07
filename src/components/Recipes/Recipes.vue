<template>
  <div class="container">
    <div class="recipes">
      <div class="_left">
        <div class="subtitle">DIY Puzzle Recipes</div>
        <h2>
          Make it, <br />
          your own.
        </h2>
        <p>
          We send you prepped ingredients for your favourite meals, all you need
          to do is cook and have fun.
        </p>
      </div>
      <div class="_right">
        <button class="cta"><a href="#">See all recipes</a></button>
      </div>
    </div>
  </div>
  <div class="recipes_flow">
    <Recipe
      v-for="recipe in recipes"
      :key="recipe.recipe"
      :img="recipe.img"
      :side="recipe.side"
      :time="recipe.time"
      :recipe="recipe.recipe"
    />
  </div>
</template>

<script>
import Recipe from "./Recipe.vue";
import { ref } from "vue";

export default {
  name: "Recipes",
  components: {
    Recipe,
  },
  setup() {
    const recipes = ref([
      {
        img: "groun-beef",
        recipe: "Grass-Fed Ground Beef & Black Bean Chili",
        side: "with Sweet Potatoes",
        time: "40 mins",
      },
      {
        img: "stuffing",
        recipe: "Herbed Sausage Stuffing",
        side: "with Onion & Celery",
        time: "40 mins",
      },
      {
        img: "bacon",
        recipe: "Baked Bacon Pizza",
        side: "with Salad",
        time: "40 mins",
      },
    ]);
    return { recipes };
  },
};
</script>
<style lang="scss" src="../../styles/recipes.scss"></style>

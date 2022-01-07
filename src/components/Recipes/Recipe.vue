<template>
  <div class="recipe">
    <div class="recipe_img">
      <img :src="require(`../../assets/${img}.png`)" />
    </div>
    <div class="recipe_details">
      <h3>{{ recipe }}</h3>
      <p>{{ side }}</p>
    </div>
    <div class="recipe_time">{{ time }} prep time</div>
  </div>
</template>

<script>
export default {
  name: "Recipe",
  props: {
    img: String,
    recipe: String,
    side: String,
    time: String,
  },
};
</script>
<style lang="scss" src="../../styles/recipe.scss"></style>

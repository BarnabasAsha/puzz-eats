<template>
  <div class="meal_plan">
    <div class="meal_plan_img">
      <img :src="require(`../../assets/${img}.png`)" />
    </div>
    <div class="meal_plan_details">
      <h3>{{ day }}</h3>
      <p>{{ meal }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "MealPlan",
  props: {
    img: String,
    day: String,
    meal: String,
  },
};
</script>

<style lang="scss" src="../../styles/MealPlan.scss"></style>

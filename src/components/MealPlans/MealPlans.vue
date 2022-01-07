<template>
  <div class="container">
    <div class="meal_plans">
      <div class="_left">
        <div class="subtitle">Weekly Meal Plans</div>
        <h2>
          Every day, <br />
          New Meals.
        </h2>
        <p>
          Set up your meal plan by saving this week's or creating an all new
          plan based on your preferences
        </p>
      </div>
      <div class="_right">
        <button class="cta-outline">
          <a href="#">Save Week's Plan</a>
        </button>
        <button class="cta"><a href="#">View all meals</a></button>
      </div>
    </div>
  </div>
  <div class="meal_plans_flow">
    <MealPlan
      v-for="meal in meals"
      :key="meal.day"
      :img="meal.img"
      :day="meal.day"
      :meal="meal.meal"
    />
  </div>
</template>

<script>
import MealPlan from "./MealPlan.vue";
import { ref } from "vue";
export default {
  name: "MealPlans",
  components: {
    MealPlan,
  },
  setup() {
    const meals = ref([
      {
        img: "monday",
        day: "Monday",
        meal: "Sweet Potato-Black Bean Tacos",
      },
      {
        img: "tuesday",
        day: "Tuesday",
        meal: "Steak & Corn Tostadas with Pickled Jalapeños:",
      },
      {
        img: "wednesday",
        day: "Wednesday",
        meal: "Kung Pao Chicken",
      },
      {
        img: "thursday",
        day: "Thursday",
        meal: "Hoisin Beef & Rice Bowl",
      },
      {
        img: "tuesday",
        day: "Friday",
        meal: "Low-Cal Cilantro-Lime Grilled Chicken",
      },
    ]);

    return { meals };
  },
};
</script>

<style lang="scss" src="../../styles/MealPlans.scss"></style>

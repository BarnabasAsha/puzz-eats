<template>
  <div class="container">
    <div class="footer">
      <FooterItem
        v-for="item in items"
        :key="item.title"
        :title="item.title"
        :list="item.list"
      />
    </div>
  </div>
</template>

<script>
import { ref } from "vue";
import FooterItem from "./FooterItem.vue";

export default {
  name: "Footer",
  components: {
    FooterItem,
  },
  setup() {
    const items = ref([
      {
        title: "Learn More",
        list: ["How It Works", "Terms And Conditions"],
      },
      {
        title: "Meal Plans",
        list: ["This Week", "Last Week"],
      },
      {
        title: "Diet Options",
        list: ["Vegan", "Low Carb", "Gluten Free"],
      },
      {
        title: "Recipes",
        list: ["Puzz Eats Rec", "Community Rec"],
      },
      {
        title: "Community",
        list: ["Join Community"],
      },
    ]);
    return { items };
  },
};
</script>

<template>
  <div class="footer_item">
    <h2>{{ title }}</h2>
    <ul>
      <li v-for="(item, index) in list" :key="index">
        <a href="#">{{ item }}</a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "FooterItem",
  props: {
    title: String,
    list: Array,
  },
};
</script>

<style lang="scss" src="../../styles/footer.scss"></style>

<template>
  <div class="option">
    <div class="option_img">
      <img :src="require(`../../assets/${img}.png`)" />
    </div>
    <div class="option_title">
      <h3>{{ title }}</h3>
      <div class="option_title_arrow">
        <img src="../../assets/arrow-right.svg" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Option",
  props: {
    img: String,
    title: String,
  },
};
</script>

<style lang="scss" src="../../styles/option.scss"></style>

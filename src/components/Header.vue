<template>
  <header>
    <div class="container">
      <div class="header">
        <div class="logo">
          <img src="../assets/puzz-eats.png" alt="Puzz eats" />
        </div>
        <div class="_right">
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
          </nav>
          <button class="cta"><a href="#">Create Meal Plan</a></button>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss" src="../styles/header.scss"></style>

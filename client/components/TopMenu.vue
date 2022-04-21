<template>
  <div class="topMenu">
    <div class="d-flex justify-content-center align-items-center">
      <nuxt-link to="/">Starters</nuxt-link>
      <span class="dot mx-3"><i class="bi bi-circle-fill"></i></span>
      <nuxt-link to="/lunch">Lunch</nuxt-link>
      <span class="dot mx-3"><i class="bi bi-circle-fill"></i></span>
      <nuxt-link to="/desserts">Desserts</nuxt-link>
      <span class="dot mx-3"><i class="bi bi-circle-fill"></i></span>
      <nuxt-link to="/yourorder"
        >Your Order
        <i class="bi bi-bag"></i>
        (0)</nuxt-link
      >
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
.topMenu {
  margin: 42px auto;
  .goldenline {
    &::after {
      display: block;
      content: '';
      height: 1px;
      width: 80%;
      margin: auto;
      background-color: goldenrod;
      position: relative;
      top: 10px;
    }
  }
  a {
    color: #6c757d;
    text-transform: uppercase;
    text-decoration: none;
    font-size: 20px;
    letter-spacing: 2px;
    border-bottom: 1px solid transparent;
    &.nuxt-link-exact-active {
      border-bottom: 1px solid goldenrod;
      @extend .goldenline;
    }
    &:hover {
      border-bottom: 1px solid goldenrod;
      @extend .goldenline;
    }
  }
  .dot {
    color: goldenrod;
    font-size: 10px;
  }
}
</style>

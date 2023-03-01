<script>
export default {

}

</script>

<template>
  <footer>
    <div class=" calltoaction">
      <div class="container">
        <ul class="menu-calltoaction">
          <li class="item_calltoaction">
            <img src="/img/buy-comics-digital-comics.png" alt="">
          </li>
          <li class="item_calltoaction">
            <img src="/img/buy-comics-merchandise.png" alt="">
          </li>
          <li class="item_calltoaction">
            <img src="/img/buy-comics-subscriptions.png" alt="">
          </li>
          <li class="item_calltoaction">
            <img src="/img/buy-comics-shop-locator.png" alt="">
          </li>
          <li class="item_calltoaction">
            <img src="/img/buy-dc-power-visa.svg" alt="">
          </li>
        </ul>
      </div>
    </div>
    <div class="menu-link">
      <ul></ul>
      <ul></ul>
      <ul></ul>
      <ul></ul>
    </div>
    <div class="community">
      <div class="community_signup">

      </div>
      <div class="community_social">
        <ul>
          <li></li>
          <li></li>
          <li></li>
          <li></li>
          <li></li>
          <li></li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use '../style/partials/variable' as *;
@use '../style/general.scss' as *;


.menu-calltoaction {
  display: flex;
  align-items: center;
}

.item_calltoaction {
  flex-basis: calc(100%*(8/12));

  &img {
    width: 100px;
  }
}

.calltoaction {
  background-color: blue;
}
</style>
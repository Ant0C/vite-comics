<script>
export default {

}

</script>

<template>
  <header class="container">
    <div class="row">
      <div class="cols">
        <img src="/img/dc-logo.png" alt="">
      </div>
      <div class="cols">
        <ul class="menu-link">
          <li class="active_link">
            <a href="#">
              CHARACTERS
            </a>
          </li>
          <li class="active_link">
            <a href="#">
              COMICS
            </a>
          </li>
          <li class="active_link active">
            <a href="#">
              MOVIES
            </a>
          </li>
          <li class="active_link">
            <a href="#">
              TV
            </a>
          </li>
          <li class="active_link">
            <a href="#">
              GAMES
            </a>
          </li>
          <li class="active_link">
            <a href="#">
              COLLECTIBLES
            </a>
          </li>
          <li class="active_link">
            <a href="#">
              VIDEOS
            </a>
          </li>
          <li class="active_link">
            <a href="#">
              FANS
            </a>
          </li>
          <li class="active_link">
            <a href="#">
              NEWS
            </a>
          </li>
          <li class="active_link">
            <a href="#">
              SHOP
            </a>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use '../style/partials/variable' as *;
@use '../style/general.scss' as *;

.row {
  align-items: center;
  justify-content: space-between;
}

.cols {
  flex-basis: 20%;
}

.menu-link {
  display: flex;
  gap: 15px;

  & li {
    padding: 42px 0px;
  }
}

.active_link:hover,
.active {
  color: $color-active-link;
  border-bottom: 4px solid $color-active-link;
}
</style>
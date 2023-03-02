<script>
export default {

}

</script>

<template>
  <section class="jumbotron">
    <span class="tag font">
      CURRENT SERIES
    </span>
  </section>
  <section class="main">
    <div class="container">
      <p class="content">
        Content goes Here
      </p>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../style/partials/variable' as *;
@use '../style/general.scss' as *;

.jumbotron {
  background-image: url('/img/jumbotron.jpg');
  background-position: top center;
  min-height: 400px;
  position: relative;
}

.tag {
  color: white;
  background-color: $color-active-link;
  padding: 15px;
  position: absolute;
  top: 95%;
  left: 21%;

}

.main {
  padding: 40px;
  background-color: #1C1C1C;
}

.content {
  color: white;
}
</style>
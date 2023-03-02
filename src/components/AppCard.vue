<script>
export default {
  props: {
    series: String,
    thumb: String,
  }
}

</script>

<template>
  <div class="card">
    <img :src="thumb" class="thumb" alt="">
    <h3 class="fontlight card_title">{{ series }}</h3>
  </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variable' as *;
@use '../style/general.scss' as *;

.card {
  padding: 15px;
}

.thumb {
  width: 150px;
  aspect-ratio: 1;
  object-fit: cover;
}

.card_title {
  margin-top: 5px;
  font-size: 14px;
  color: white;
}
</style>
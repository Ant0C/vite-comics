<script>
export default {

}

</script>

<template>
  <main>
    <div class="container">
      <p class="content">
        Content goes Here
      </p>
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use '../style/partials/variable' as *;
@use '../style/general.scss' as *;

main {
  padding: 40px;
  background-color: black;
}

.content {
  color: white;
}
</style>
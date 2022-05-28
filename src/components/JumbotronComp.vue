<template>
  <div class="jumbotron">
    <div class="container">
      <div class="row">
        <div class="col-6">1</div>
        <div class="col-6 cd">
          <img src="../assets/images/Group-35-2x.png" alt="jumbotron-pic-1">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'JumbotronComp'
}
</script>

<style lang="scss" scoped>

.jumbotron {
  overflow: hidden;
  height: 800px;
}
  .col-6.cd {
    img {
      position: relative;
      top: -170px;
      right: 250px;
      width: 210%;
    }
    }


</style>
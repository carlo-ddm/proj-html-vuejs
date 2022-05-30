<template>
  <section>
    <div class="top d-flex align-items-center">
      <div class="container">
        <div class="row">
          <div class="col-6 cd1">
            <h1>ciao</h1>
          </div>
          <div class="col-6 cd2">
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aliquam adipisci ducimus animi pariatur ab, accusantium error commodi hic ut laboriosam facere dicta, assumenda quis rem ea dolores accusamus esse! Laudantium.</p>
          </div>
        </div>
      </div>
    </div>
    <div class="bottom">
      bottom
    </div>
  </section>
</template>

<script>
export default {
  name: 'SecThree'
}
</script>

<style lang="scss" scoped>
.col-6 {
  border: 1px solid black
}

section {
  width: 100%;
  height: 800px;
  .top {
    height: calc(30%);
  }
}
</style>
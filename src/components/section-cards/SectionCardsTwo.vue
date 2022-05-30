<template>
<div class="cd_card">
  <img :src="`${item.pic}`" alt="">
</div>
</template>

<script>
export default {
  name: 'SectionCardsTwo',
  props: {
    item: Object
  }
}
</script>

<style lang="scss" scoped>
.cd_card {
  flex-basis: 24.5%;
  height: 24.5%;
  margin-bottom: 10px;
  img {
    width: 100%;
  }
}

</style>
<template>
<div class="cd_card">
  <img :src="`${card.card}`" alt="">
</div>
</template>

<script>
export default {
  name: 'SectionCardsTwo',
  props: {
    card: Object
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
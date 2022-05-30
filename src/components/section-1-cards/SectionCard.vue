<template>
  <div class="cd_card">
    <i :class="`fa-solid ${cardItem.icon}`"></i>
    <h6>{{cardItem.arg}}</h6>
    <p>{{cardItem.text}}</p>
  </div>
</template>

<script>

export default {
  name: 'SectionCard',
  props: {cardItem: Object}
}
</script>

<style lang="scss" scoped>
  .cd_card {
  flex-basis: 45%;
  height: 220px;
  margin-bottom: 40px;
  border: 1px solid black;
}
</style>
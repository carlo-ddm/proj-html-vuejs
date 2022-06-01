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
@import '../../assets/styles/vars';
@import '../../assets/styles/mixines';

  .cd_card {
    padding: 35px 30px;
    flex-basis: 45%;
    height: 240px;
    margin: 0 0 20px 20px;
    border: 1px solid #FFFFFF;
    border-radius: 10px;
    box-shadow: 0 0 25px #DEDEDE;
    h6 {
      font-size: 20px;
      font-weight: 200;
      text-transform: capitalize;
    }
    
    p {
    @include paragr
  }
}
</style>
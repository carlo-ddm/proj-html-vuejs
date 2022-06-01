<template>
          <div class="cdd-box">
            <h4>designin</h4>
            <span>all designs</span>
            <div class="price-black d-flex justify-content-center align-items-center">price</div>
            <ul class="p-0">
              <li>bisosos</li>
              <li>bisosos</li>
              <li>bisosos</li>
              <li>bisosos</li>
              <li>bisosos</li>
          </ul>
          </div>
</template>

<script>
export default {
  name: 'SectionCardsThree',
  data() {
    return {
      props: {cardItem: Object}
    }
  },
}
</script>

<style lang="scss" scoped>
// import Vars
@import '../../assets/styles/vars';
// import Mixines
@import '../../assets/styles/mixines';
// import Utilities
@import '../../assets/styles/utilities.scss';

.offers {
        padding: 0 40px;

        .cdd-box {
          text-align: center;
          border: 1px solid #FFFFFF;
          border-radius: 10px;
          background-color: white;
          box-shadow: 0 0 15px #dedede;
          height: 500px;
          border-radius: 10px;
          .price-black {
            width: 100%;
            height: 80px;
            @include black-grad
          }
          .price-green {
            width: 100%;
            height: 80px;
            @include grad
          }

          ul {
            margin-top: 40px;
            li {
              @include list-style;
              justify-content: center;
              margin: 20px 0px;
              &::before {
                content: '/2713';
                display: inline-block;
                width: 12px;
                height: 12px;
                background-position: center;
                line-height: 1px;
                margin-left: 4px;
              }
            }
          } 
        }
      }

</style>
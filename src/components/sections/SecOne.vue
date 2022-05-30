<template>
  <section class="d-flex justify-content-center align-items-center">
      <div class="container">
        <div class="row">
  
          <!-- Colonna 1 -> TESTO -->
          <div class="col-6 cd1">
            <div class="cd_container">
              <div class="we-are-here">
                <h1 class="m-0">We are here to
                  <br>
                   make your website
                   <br>
                   look more elegant
                   <br>
                   and stylish
                </h1>
              </div>
              <button class="cd-btn">view all</button>
            </div>
          </div>
  
          <!-- Colonna 2 -> IMMAGINE -->
          <div class="col-6 cd2">
            <!-- CARDS -->
            <div class="wrapper d-flex flex-wrap justify-content-between">
              <SectionCard v-for="(card, index) in cards" :key="`_index_${index}`" :cardItem="card" />
            </div>
          </div>
        </div>
      </div>
    </section>
</template>

<script>
import SectionCard from "../section-cards/SectionCard.vue";
export default {
    name: "SecOne",

    data() {
      return {
        cards: [
          {
            icon: 'fa-gauge-simple-high',
            arg: 'speed optimization',
            text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. At earum quam cumque cum quod vero.'
          },
          {
            icon: 'fa-cloud',
            arg: 'cloud solution',
            text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. At earum quam cumque cum quod vero.'
          },
          {
            icon: 'fa-mobile-screen-button',
            arg: 'website design',
            text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. At earum quam cumque cum quod vero.'
          },
          {
            icon: 'fa-clock',
            arg: 'online marketing',
            text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit. At earum quam cumque cum quod vero.'
          },
        ]
      }
    },

    components: { SectionCard }
}
</script>

<style lang="scss" scoped>
//i import Vars
@import '../../assets/styles/vars';
// import Mixines
@import '../../assets/styles/mixines';
// import Utilities
@import '../../assets/styles/utilities.scss';

section {
  width: 100%;
  height: 800px;

  .col-6.cd1 {
    padding-top: 130px;

    .cd_container {
      .we-are-here {
        margin-bottom: 40px;
    }

    }


  }
}

</style>
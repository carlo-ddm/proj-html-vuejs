<template>
  <section>
    <div class="top d-flex align-items-center">
      <div class="container">
        <div class="row">
          <div class="col-6 cd1">
            <h1>our recente web design -----&---- some examples of past projects</h1>
          </div>
          <div class="col-6 cd2 d-flex align-items-center">
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aliquam adipisci ducimus animi pariatur ab, accusantium error commodi hic ut laboriosam facere dicta, assumenda quis rem ea dolores accusamus esse! Laudantium.</p>
          </div>
        </div>
      </div>
    </div>
    <div class="bottom container wrapper d-flex flex-wrap justify-content-between">
      <SectionCardsTwo v-for="(card, index) in cards" :key="`_index_${index}`" :card="card" />
    </div>
    <div class="container d-flex justify-content-center">
      <div class="cd-btn">ciao</div>
    </div>
  </section>
</template>

<script>
import SectionCardsTwo from '../section-cards/SectionCardsTwo.vue';
import img1 from '../../assets/images/ina-soulis-227104-unsplash-1024x1024.jpg';
import img2 from '../../assets/images/sunisa-misa-531163-unsplash-1024x1024.jpg';
import img3 from '../../assets/images/355H-1024x1024.jpg';
import img4 from '../../assets/images/photo-1448932252197-d19750584e56-1024x1024.jpg';
import img5 from '../../assets/images/business-competition-PB366D8-1024x1024.jpg';
import img6 from '../../assets/images/cozy-sofa-in-living-room-PQR5AB9-1024x1024.jpg';
import img7 from '../../assets/images/aa9a4539-PQGJ7HU-1024x1024.jpg';
import img8 from '../../assets/images/cody-davis-253928-unsplash-1024x1024.jpg';
export default {
    name: "SecThree",
    data() {
      return {
        cards:[
          {
            card: img1
          },
          {
            card: img2
          },
          {
            card: img3
          },
          {
            card: img4
          },
          {
            card: img5
          },
          {
            card: img6
          },
          {
            card: img7
          },
          {
            card: img8
          },
        ]
      }
    },
    components: { SectionCardsTwo }
}
</script>


<style lang="scss" scoped>
@import '../../assets/styles/utilities.scss';

// .col-6 {
//   border: 1px solid black
// }

section {
  width: 100%;
  height: 1000px;
  .top {
    height: calc(30%);
    .container {
      height: 200px;
      .col-6.cd2 {
        padding-top: 60px;
      }
    }
  }
  .cd-btn {
    display: flex;
    justify-self: center;
    background-color: bisque;
  }

}
</style>
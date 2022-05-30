<template>
  <section class="d-flex justify-content-center align-items-center">

      <div class="row">
        <div class="col-6 cd1">
          <img class="architect" src="../../assets/images/busy-architect-PYVKWM4-1024x872.jpg" alt="">
          <img class="woman" src="../../assets/images/businesswoman-analysing-document-P8WSNMC-1024x820.jpg" alt="">
        </div>
        <div class="col-6 cd2">
          <div class="cd_container">
            <div class="learn-more">
               <h1 class="m-0">learn more
                  <br>
                   about our
                   <br>
                   mission
                </h1>
                <div>
                  <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo sed, molestias corrupti ea debitis nulla consectetur nesciunt accusamus esse consequatur laudantium incidunt accusantium nihil deleniti dicta commodi, cupiditate ratione! Optio ad, cumque delectus iusto fuga dignissimos voluptas inventore nobis velit!
                  </p>
                </div>
                <button class="cd-btn">readmore</button>
            </div>
          </div>

        </div>
      </div>


  </section>
</template>

<script>
export default {
  name: 'SecTwo'
}
</script>

<style lang="scss" scoped>
@import '../../assets/styles/vars';
// import Mixines
@import '../../assets/styles/mixines';
// import Utilities
@import '../../assets/styles/utilities.scss';
section {
  width: 100%;
  height: 800px;
  background-color: #F9F9F9;

  .col-6.cd1 {
    position: relative;
    display: flex;
    align-items: center;
    img.architect {
      width: 600px;
      border-radius: 20px;
    }
    img.woman {
      position: absolute;
      left: 180px;
      top: 150px;
      width: 600px;
      border-radius: 20px;
    }
  }


  .col-6.cd2 {
    padding-top: 130px;
    padding-left: 70px;
    .cd_container {

      .learn-more {
        margin-bottom: 40px;
      }

      p {
        margin: 40px 0 40px 0px !important;
      }

       button {
        margin: 40px 0 40px 0px;
      }
    }
  }
}
</style>
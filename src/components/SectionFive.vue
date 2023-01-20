<template>
  <div class="container-fluid section5">
    <div class="row py-2">
      <div class="col-lg-6 d-flex justify-content-center align-items-center">
        <div class="div px-lg-5 px-2" data-aos="fade-up">
          <div class="title text-left mt-md-5 mt-4" >
            SIMPLE BUT EFFECTIVE GAME ECONOMIC MODEL
          </div>
          <div class="content mt-lg-5 mt-2 text-left">
            Players can earn tokens from playing the game with personal skills
            and strategies, and use the earned tokens to upgrade NFT items use
            them to play games or sell for profit.
          </div>
        </div>
      </div>
      <div class="col-lg-6">
        <SpinView data-aos="flip-left"/>
      </div>
    </div>
  </div>
</template>

<script>
import SpinView from "@/components/Spin.vue";
export default {
  name: "SectionFour",
  components: {
    SpinView,
  },
  props: {},
};
</script>
<style lang="scss" scoped>
.section5 {
  background-image: url("@/assets/img/background6.png");
  background-repeat: no-repeat;
  background-size: cover;
  .title {
    color: white;
    font-size: clamp(12px, 3.5vw, 40px);
    text-shadow: 0 0 7px #061fff, 0 0 10px #061fff, 0 0 21px #061fff,
      0 0 42px #061fff, 0 0 82px #061fff;
    @media (max-width: 768px) {
      font-size: 18px;
    }
  }
  .content {
    color: white;
    font-size: clamp(12px, 3.5vw, 20px);
  }
}
</style>

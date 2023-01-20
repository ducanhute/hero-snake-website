<template>
  <div>
    <div class="container-fluid section2">
      <div class="row">
        <div class="title col-12 text-white font-weight-bold" data-aos="fade-up">game play</div>
        <div class="content col-12 text-white" data-aos="fade-up">
          <p class="description">
            At Hero Snake, all you have to do is eat, survive, fight. You will
            have to control your Snake to fly in the Space Room, eat stars and
            galaxies to increase size and level, dodge or destroy other
            opponents.
          </p>
        </div>

        <div class="image col-12"  data-aos="zoom-in-down">
          <img src="@/assets/img/section2img1.jpg" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "SectionTwo",
  props: {},
};
</script>
<style lang="scss" scoped>
.section2 {
  padding: 60px 0 180px 0;
  background-image: url("@/assets/img/background3.png");
  background-repeat: no-repeat;
  @media (max-width: 991px) {
    padding: 60px 0 100px 0;
  }
  .title {
    text-transform: uppercase;
    font-size: clamp(30px, 3.5vw, 60px);
    // font-size: 40px;
    line-height: 150%;
    margin-bottom: 20px;
    text-shadow: 0 0 7px #e31b1b, 0 0 10px #e31b1b, 0 0 21px #e31b1b,
      0 0 42px #e31b1b, 0 0 82px #e31b1b, 0 0 92px #e31b1b, 0 0 102px #e31b1b,
      0 0 151px #e31b1b;
  }
  .content {
    display: flex;
    justify-content: center;
  }
  .description {
    width: 60%;
    font-size: clamp(10px, 3.5vw, 30px);
  }
  .image {
    margin: auto;
    margin-top: 20px;
    max-width: 828px;
    width: 100%;
    img {
      width: 100%;
      object-fit: scale-down;
      @media (max-width: 991px) {
        width: 90%;
      }
    }
  }
}
</style>

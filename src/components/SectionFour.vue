<template>
  <div class="container-fluid section4">
    <div class="row py-5 align-items-center">
      <div class="image col-12 col-lg-6 col-md-12" data-aos="flip-left">
        <img src="@/assets/img/section4.png" alt="" />
      </div>
      <div class="col-12 col-lg-6 col-md-12">
        <div class="title font-weight-bold"  data-aos="fade-up">evolution</div>
        <ul class="content"  data-aos="fade-up">
          <li class="my-lg-5 my-md-3 my-2">
            Snake levels will be raised based on the number of tokens earned
            from battles and the number of battles you participate in.
          </li>
          <li class="my-lg-5 my-md-3 my-2">
            Through each battle your snake will gain more experience to upgrade,
            grow in size and dominate the room.
          </li>
          <li class="my-lg-5 my-md-3 my-2">
            Equip the items available in the Marketplace to increase the
            advantage of earning more HBG tokens.
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "SectionFour",
  props: {},
};
</script>
<style lang="scss" scoped>
.section4 {
  background-image: url("@/assets/img/background5.png");
  background-repeat: no-repeat;
  background-size: cover;
  .image {
    width: 100%;
    img {
      width: 100%;
      object-fit: scale-down;
    }
  }
  .title {
    font-size: 40px;
    color: white;
    text-transform: uppercase;
    text-shadow: 0 0 7px #061fff, 0 0 10px #061fff, 0 0 21px #061fff,
      0 0 42px #061fff, 0 0 82px #061fff;
  }

  .content {
    list-style: url("@/assets/img/icon1.svg");
    color: white;
    font-size: clamp(12px, 4vw, 24px);
    text-align: left;
    padding: 16px 0;
    @media (max-width: 991px) {
      padding-left: 40px;
    }
    @media (max-width: 767px) {
      padding: 0px 0;
      padding-left: 40px;
    }
  }
}
</style>

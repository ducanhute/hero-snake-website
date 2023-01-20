<template>
  <div class="container-fluid section3">
    <div class="title text-white font-weight-bold" data-aos="fade-up">
      FUN TO EARN
    </div>
    <div class="row">
      <div class="col-12 col-lg-5 col-md-5">
        <div class="img1" data-aos="zoom-in-right">
          <img src="@/assets/img/snake4.png" alt="" />
        </div>
      </div>
      <div class="img1-des col-12 col-lg-7 col-md-7" data-aos="fade-up">
        <ul class="heading text-white font-weight-bold">
          Survival
          <li class="heading-item">
            Defeat the enemy snake, protect your snake and proceed to the safe
            door
          </li>
          <li class="heading-item">
            Safe Doors: These are exit-like portals that you can use to exit the
            game without losing your snake/NFT. They appear randomly and don't
            last long so watch out and act fast
          </li>
        </ul>
      </div>
    </div>
    <div class="row mt-40">
      <div class="img1-des col-12 col-lg-6 col-md-6" data-aos="fade-up">
        <ul class="mt-40 ml heading text-white font-weight-bold">
          Defeat is not the end:
          <li class="heading-item">
            When your snake is defeated, don't worry because you will still
            receive a portion of the tokens earned in the battle room 10% will
            Part of the token will be scattered right where you are defeated
          </li>
          <li class="heading-item">go to the person who beat you</li>
          <li class="heading-item">
            Part of the token will be scattered right where you are defeated
          </li>
        </ul>
      </div>
      <div
        class="col-12 col-lg-6 col-md-6 p-relative text-right"
        data-aos="zoom-in-left"
      >
        <div class="plannet">
          <img src="@/assets/img/planet.png" alt="" />
        </div>
        <div class="img2">
          <img src="@/assets/img/snake 3.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "SectionThree",
  props: {},
};
</script>
<style lang="scss" scoped>
.mt-40 {
  margin-top: 40px;
}
.ml {
  margin-left: 100px;
  @media (max-width: 991px) {
    margin-left: 0px;
    margin-bottom: 40px;
  }
}
.p-relative {
  position: relative;
}
.plannet {
  position: absolute;
  top: 10%;
  left: 0%;
  animation: example 2s linear 3s infinite alternate;

  @media (max-width: 991px) {
    top: 30%;
    left: 15%;
    animation: example1 2s linear 3s infinite alternate;
  }
  @media (max-width: 767px) {
    top: -10%;
    left: 12%;
    animation: example2 2s linear 3s infinite alternate;
  }

  @media (max-width: 991px) {
    img {
      width: 150px;
      height: 150px;
    }
  }
}
@keyframes example {
  from {
    top: 10%;
  }
  to {
    top: 30%;
  }
}
@keyframes example1 {
  from {
    top: 30%;
  }
  to {
    top: 40%;
  }
}
@keyframes example2 {
  from {
    top: -10%;
  }
  to {
    top: 20%;
  }
}
.section3 {
  background-image: url("@/assets/img/background4.png");
  background-repeat: no-repeat;
  background-size: cover;
  .title {
    font-size: 32px;
    margin-bottom: 100px;
    text-shadow: 0 0 7px #ffb906, 0 0 10px #ffb906, 0 0 21px #ffb906,
      0 0 42px #ffb906, 0 0 82px #ffb906;
    @media (max-width: 768px) {
      margin-bottom: 20px;
    }
  }

  .img1 {
    max-width: 654px;
    width: 100%;
    text-align: left;
    margin-left: -20px;
    img {
      margin-top: -260px;
      width: 80%;
      object-fit: scale-down;
      @media (max-width: 767px) {
        margin-top: 0;
        width: 100%;
      }
    }
  }
  .img2 {
    max-width: 654px;
    width: 100%;
    float: right;
    margin-right: -20px;
    img {
      margin-top: 200px;
      width: 60%;
      object-fit: scale-down;
      @media (max-width: 767px) {
        margin-top: 20px;
      }
    }
  }
  .heading {
    list-style: url("@/assets/img/icon1.svg");
    font-size: 30px;
    text-transform: uppercase;
    text-align: left;
    text-shadow: 0 0 7px #ff12cb, 0 0 10px #ff12cb, 0 0 21px #ff12cb,
      0 0 42px #ff12cb, 0 0 82px #ff12cb, 0 0 92px #ff12cb;
    .heading-item {
      font-size: 20px;
      margin: 10px 0;
      text-transform: initial;
      font-weight: 500;
      text-shadow: none;
    }
  }
}
</style>

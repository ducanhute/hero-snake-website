<template>
  <div class="section6">
    <div class="container">
      <div class="title text-white pt-3 pt-sm-4" data-aos="fade-up">
        DIFFERENT WAYS TO EARN TOKEN
      </div>
      <div class="row justify-content-center py-lg-5" data-aos="fade-up">
        <div class="item col-10 col-sm-5 box-shadow1 mx-3 my-4 border">
          <div class="heading my-2 my-sm-3 my-md-2">purchase</div>
          <div class="content text-white">
            You can buy and sell HeroBox, try your luck by opening HeroBox to
            hunt rare NFTs and sell them. Or raise snakes to a higher level,
            sell snakes and items on Marketplace for a profit.
          </div>
        </div>
        <div class="item col-10 col-sm-5 box-shadow2 mx-3 my-4 border">
          <div class="heading my-2 my-sm-3 my-md-2">gaming</div>
          <div class="content text-white">
            You can buy and sell HeroBox, try your luck by opening HeroBox to
            hunt rare NFTs and sell them. Or raise snakes to a higher level,
            sell snakes and items on Marketplace for a profit.
          </div>
        </div>
        <div class="item col-10 col-sm-5 box-shadow3 mx-3 my-4 border">
          <div class="heading my-2 my-sm-3 my-md-2">Bonus hunting</div>
          <div class="content text-white">
            Participate in monthly and weekly events, perform daily tasks,
            compete for positions in the gold table, you will receive attractive
            rewards.
          </div>
        </div>
        <div class="item col-10 col-sm-5 box-shadow4 mx-3 my-4 border">
          <div class="heading my-2 my-sm-3 my-md-2">INTRODUCE</div>
          <div class="content text-white">
            Invite your friends to play the game, you will receive a commission
            corresponding to 0.1% of the value they earn.
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionSix",
  props: {},
};
</script>
<style lang="scss" scoped>
.box-shadow1 {
  box-shadow: 0 0 2px #6df9b5, 0 0 10px #6df9b5, 0 0 20px #6df9b5;
  .heading {
    color: #6df9b5;
  }
}
.box-shadow2 {
  box-shadow: 0 0 2px #f96d80, 0 0 10px #f96d8b, 0 0 20px #f96d74;
  .heading {
    color: #f96d80;
  }
}
.box-shadow3 {
  box-shadow: 0 0 2px #e912ba, 0 0 10px #f132a8, 0 0 20px #f03dc9;
  .heading {
    color: #e912ba;
  }
}
.box-shadow4 {
  box-shadow: 0 0 2px #f9c86d, 0 0 10px #f9f06d, 0 0 20px #f9f76d;
  .heading {
    color: #f9f06d;
  }
}

.section6 {
  background-image: url("@/assets/img/background7.png");
  background-repeat: no-repeat;
  background-size: cover;
  .item {
    min-height: 200px;
    @media (max-width: 576px) {
      min-height: 130px;
    }
  }
  .title {
    font-size: clamp(12px, 3.5vw, 40px);
    text-shadow: 0 0 7px #061fff, 0 0 10px #061fff, 0 0 21px #061fff,
      0 0 42px #061fff, 0 0 82px #061fff;

    @media (max-width: 768px) {
      font-size: 18px;
    }
  }
  .heading {
    font-size: clamp(12px, 3.5vw, 30px);
    text-transform: uppercase;
    font-weight: 600;
  }
  .content {
    font-size: clamp(10px, 3.5vw, 20px);
  }
  .border {
    border-radius: 15px;
  }
}
</style>

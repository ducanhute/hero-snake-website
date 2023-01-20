<template>
  <div class="section7 py-5 py-lg-4">
    <!-- Title -->
    <div class="title text-white pt-3 pt-sm-4" data-aos="fade-up">
      WHY SHOULD JOIN HERO SNAKE?
    </div>
    <div
      class="d-lg-none py-4 d-flex justify-content-center align-items-center"
      data-aos="fade-right"
    >
      <img class="logo" src="@/assets/img/section7Logo.png" alt="" />
    </div>
    <!-- body -->
    <div class="row justify-content-center">
      <div
        class="item1 col-lg-3 col-10 col-md-5 text-left"
        data-aos="fade-right"
      >
        <div class="s1">
          <div class="text-danger font-weight-bold mt-4">
            TOP BLOCKCHAIN FOUNDATION
          </div>
          <div class="text-white mt-1">
            Built on the Binance Smart Chain platform, assets move quickly
            between networks and transaction costs are competitive
          </div>
        </div>
        <div class="s2">
          <div class="text-success font-weight-bold mt-4">
            HUGE INCOME INCREASE
          </div>
          <div class="text-white mt-1">
            With your training, the snakes gradually evolve to higher levels,
            which means that the NFT value is also more scarce, thereby bringing
            great profits to you.
          </div>
        </div>
        <div class="s3">
          <div class="text-primary font-weight-bold mt-4">
            TOP BLOCKCHAIN FOUNDATION
          </div>
          <div class="text-white mt-1">
            Using blockchain technology to help prevent censorship and
            interference from publishers
          </div>
        </div>
      </div>

      <div
        class="
          item2
          col-5
          d-lg-flex d-none
          align-item-center
          justify-content-center
        "
        data-aos="fade-up"
      >
        <div class="row w-100 h-100">
          <div class="f1 col-md-3">
            <div class="row w-100 h-100">
              <div
                class="
                  pt-5
                  px-0
                  d-flex
                  align-items-end
                  justify-content-center
                  col-12
                "
              >
                <div class="tree">
                  <img src="@/assets/img/tree1.png" alt="" />
                </div>
              </div>

              <div
                class="
                  pt-5
                  px-0
                  d-flex
                  align-items-end
                  justify-content-center
                  col-12
                "
              >
                <div class="tree">
                  <img src="@/assets/img/tree2.png" alt="" />
                </div>
              </div>

              <div
                class="
                  px-0
                  d-flex
                  align-items-start align-items-xl-center
                  justify-content-center
                  col-12
                "
              >
                <div class="tree">
                  <img src="@/assets/img/tree3.png" alt="" />
                </div>
              </div>
            </div>
          </div>
          <div
            class="f2 col-6 d-flex align-items-center justify-content-center"
          >
            <img class="logo" src="@/assets/img/section7Logo.png" alt="" />
          </div>

          <div class="f3 col-md-3">
            <div class="row w-100 h-100">
              <div
                class="
                  pt-5
                  px-0
                  d-flex
                  align-items-end
                  justify-content-center
                  col-12
                "
              >
                <div class="tree">
                  <img src="@/assets/img/tree4.png" alt="" />
                </div>
              </div>

              <div
                class="
                  pt-5
                  px-0
                  d-flex
                  align-items-end
                  justify-content-center
                  col-12
                "
              >
                <div class="tree">
                  <img src="@/assets/img/tree5.png" alt="" />
                </div>
              </div>

              <div
                class="
                  px-0
                  d-flex
                  align-items-start align-items-xl-center
                  justify-content-center
                  col-12
                "
              >
                <div class="tree">
                  <img src="@/assets/img/tree6.png" alt="" />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div
        class="item3 col-lg-3 col-10 col-md-5 text-left"
        data-aos="fade-left"
      >
        <div class="s4">
          <div class="text-info font-weight-bold mt-4">HUGE ECOSYSTEM</div>
          <div class="text-white mt-1">
            The solid Herocoin ecosystem is a sure springboard for Hero Snake to
            develop
          </div>
        </div>
        <div class="s5">
          <div class="font-weight-bold mt-4 text-danger">STRONG TOKEN</div>
          <div class="text-white mt-1">
            HBG token with limitless upside potential thanks to high liquidity
            in HEROBOOK's vast ecosystem.
          </div>
        </div>
        <div class="s6">
          <div class="font-weight-bold mt-4 text-success">AWESOME GAMEPLAY</div>
          <div class="text-white mt-1">
            Gameplay is simple but requires high tactics to create an engaging
            and engaging experience
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionSeven",
  props: {},
};
</script>
<style lang="scss" scoped>
.section7 {
  background-image: url("@/assets/img/background7.png");
  background-repeat: no-repeat;
  background-size: cover;
  .title {
    font-size: clamp(16px, 3.5vw, 40px);
    text-shadow: 0 0 7px #be06ff, 0 0 10px #be06ff, 0 0 21px #be06ff,
      0 0 42px #be06ff, 0 0 52px #be06ff, 0 0 62px #be06ff;

    @media (max-width: 768px) {
      font-size: 30px;
    }
    @media (max-width: 576px) {
      font-size: 20px;
    }
  }
  .item2 {
    .logo {
      width: 100%;
      object-fit: scale-down;
    }
    .tree {
      max-width: 180px;
      width: 100%;
      img {
        width: 140%;
        object-fit: scale-down;
      }
    }
  }
}
</style>

<template>
  <div class="section1 container-fluid">
    <div class="row minus-margin justify-content-around">
      <div
        v-for="item in content"
        :key="item"
        class="col-3 wrap-sologan"
        data-aos="flip-left"
      >
        <div class="sologan">
          <div :class="item.shadow" class="title-sologan p-relative">
            {{ item.title }}
          </div>
          <div class="title-des p-relative2">{{ item.des }}</div>
        </div>
      </div>
    </div>
    <div class="row py-5 mobile-height align-items-center h-100">
      <div class="image col-lg-6 col-md-12 col-sm-12">
        <div class="img1" data-aos="zoom-in">
          <img src="@/assets/img/snack.png" alt="" />
        </div>
      </div>
      <div class="content col-lg-6 col-md-12 col-sm-12" data-aos="fade-up">
        <div class="title text-left font-weight-bold text-white">
          {{ title }}
        </div>
        <ul class="subtitle text-left font-weight-bold text-white">
          {{
            subTitle
          }}
          <li class="subtitle-item">{{ content1 }}</li>
          <li class="subtitle-item">{{ content2 }}</li>
          <li class="subtitle-item">{{ content3 }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionOne",
  props: {},
  data() {
    return {
      title: "HERO SNAKE",
      subTitle: "Coming from the HEROCOIN ecosystem",
      content1:
        "Hero Snake is a next project in the vast ecosystem of HEROCOIN",
      content2:
        "Hero Snake is a game that completely combines the NFT game platform and the arcade game from the Herocoin ecosystem, using the HBG token and built on the Binance Smart Chain (BSC) platform.",
      content3:
        "Help players earn income with fun gaming experience and personal skills and strategies",
      content: [
        {
          title: "play to earn",
          des: "Fight - survive to get the Tokens for yourself",
          shadow: "text-shadow1",
        },
        {
          title: "play to earn",
          des: "Fight - survive to get the Tokens for yourself",
          shadow: "text-shadow2",
        },
        {
          title: "play to earn",
          des: "Fight - survive to get the Tokens for yourself",
          shadow: "text-shadow3",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.section1 {
  background-image: url("@/assets/img/background2.png");
  background-repeat: no-repeat;
  background-size: cover;
  // height: 100vh;
  .wrap-sologan {
    background: #122448;
    padding: 20px 5px;
    border-radius: 8px;
    margin-top: -60px;
  }
  .p-relative {
    position: relative;
    &::before {
      content: url(@/assets/img/sword1.svg);
      position: absolute;
      top: 0;
      left: 10%;
      @media (max-width: 1150px) {
        display: none;
      }
    }
    &::after {
      content: url(@/assets/img/sword2.svg);
      position: absolute;
      top: 0;
      left: 10%;
      @media (max-width: 1150px) {
        display: none;
      }
    }
  }
  .p-relative2 {
    position: relative;
    &::after {
      content: url(@/assets/img/sword2.svg);
      position: absolute;
      top: -94%;
      left: 84%;
      @media (max-width: 1150px) {
        display: none;
      }
    }
    &::before {
      content: url(@/assets/img/sword1.svg);
      position: absolute;
      top: -94%;
      left: 84%;
      @media (max-width: 1150px) {
        display: none;
      }
    }
  }
  border-radius: 8px;
  .title-sologan {
    text-transform: uppercase;
    font-size: 22px;
    color: white;
    margin-bottom: 10px;
    @media (max-width: 576px) {
      font-size: 14px;
    }
  }
  .text-shadow1 {
    text-shadow: 0 0 7px #ff0101, 0 0 10px #ff0101, 0 0 21px #ff0101,
      0 0 42px #ff0101, 0 0 82px #ff0101;
  }
  .text-shadow2 {
    text-shadow: 0 0 7px #0bf9ea, 0 0 10px #0bf9ea, 0 0 21px #0bf9ea,
      0 0 42px #0bf9ea, 0 0 82px #0bf9ea;
  }
  .text-shadow3 {
    text-shadow: 0 0 7px #0046f9, 0 0 10px #0046f9, 0 0 21px #0046f9,
      0 0 42px #0046f9, 0 0 82px #0046f9;
  }
  .title-des {
    text-transform: uppercase;
    font-size: 16px;
    color: white;
    @media (max-width: 576px) {
      font-size: 10px;
    }
  }
  .mobile-height {
    @media (max-width: 576px) {
      height: 400px;
    }
  }
}
.image {
  .img1 {
    max-width: 620px;
    width: 100%;
    img {
      width: 100%;
      object-fit: scale-down;
      margin: auto;
    }
  }
}

.title {
  font-size: 40px;
  padding-bottom: 20px;
  text-shadow: 0 0 7px #8b1be3, 0 0 10px #8b1be3, 0 0 21px #8b1be3,
    0 0 42px #8b1be3, 0 0 82px #8b1be3;
  @media (max-width: 576px) {
    font-size: 30px;
  }
}
.subtitle {
  font-size: 30px;
  margin-bottom: 20px;
  list-style: square inside url("@/assets/img/icon1.svg");
  @media (max-width: 576px) {
    font-size: 20px;
  }
  .subtitle-item {
    //font-size with width change
    font-size: clamp(14px, 2.5vw, 26px);
    line-height: 150%;
    font-weight: 500;
    padding: 10px;
  }
}
.content {
  font-size: 20px;
  @media (max-width: 576px) {
    font-size: 14px;
  }
}
</style>

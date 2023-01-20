<template>
  <div class="section8 py-lg-5 py-md-5 py-2">
    <!-- row-all -->
    <div class="row">
      <!-- col-2-all -->
      <div class="col-4 d-md-none"></div>
      <div class="col-md-2 col-8 pr-5 pr-md-0" data-aos="fade-right">
        <div class="title text-white font-weight-bold">ROAD MAP</div>
        <div class="display-mobile d-md-none">
          <div class="phase1 box-s1 pt-2 my-4">
            <div class="heading s1 font-weight-bold">PHASE1</div>
            <p class="content-heading">Alpha Test</p>
          </div>
          <div class="phase2 box-s2 pt-2 my-4">
            <div class="heading s2 font-weight-bold">PHASE2</div>
            <p class="content-heading">Close beta test Open beta test</p>
          </div>
          <div class="phase3 box-s3 pt-2 my-4">
            <div class="heading s3 font-weight-bold">PHASE3</div>
            <p class="content-heading">
              Release new snakes. Organize tournaments Open multinational
              tournaments.
            </p>
          </div>
          <div class="phase4 box-s4 pt-2 my-4">
            <div class="heading s4 font-weight-bold">PHASE4</div>
            <p class="content-heading">Release the official game version</p>
          </div>
        </div>
        <div class="title-image d-none d-md-block">
          <img src="@/assets/img/section8Img1.png" alt="" />
        </div>
      </div>
      <!-- col-10-all -->
      <div class="col-10 d-none d-md-block" data-aos="fade-up">
        <!-- ------------------ -->
        <div class="row">
          <div class="col-6">
            <div class="row">
              <div class="col-6 p-relative">
                <div class="planet1 img-style p-relative">
                  <img src="@/assets/img/section8Img2.png" alt="" />
                </div>
              </div>
              <div
                class="des-one col-6 option-padding p-relative text-left pl-5"
              >
                <div class="heading text font-weight-bold">PHASE 1</div>
                <p class="sub-text">Alpha Test</p>
              </div>
            </div>
          </div>

          <div class="col-6">
            <div class="row">
              <div class="col-6 p-relative">
                <div class="galaxy img-style p-relative">
                  <img src="@/assets/img/section8Img4.png" alt="" />
                </div>
              </div>
              <div class="col-6">
                <div class="des-one option-padding p-relative text-left pl-5">
                  <div class="heading text font-weight-bold">PHASE 2</div>
                  <span class="sub-text">Close beta test</span>
                  <p class="sub-text">Open beta test</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!--  -->
        <div class="row padding">
          <div class="col-6">
            <div class="row">
              <div class="col-6 p-relative">
                <div class="cup img-style">
                  <img src="@/assets/img/section8Img3.png" alt="" />
                </div>
              </div>
              <div class="des-one col-6 p-relative pl-4">
                <div class="heading text font-weight-bold">PHASE 4</div>
                <p class="sub-text ml-2">
                  Release new snakes. Organize tournaments Open multinational
                  tournaments.
                </p>
              </div>
            </div>
          </div>

          <div class="col-6">
            <div class="row">
              <div class="col-6">
                <div class="des-two p-relative text-left ml-5">
                  <div class="heading text font-weight-bold">PHASE 3</div>
                  <p class="sub-text">Release the official game version</p>
                </div>
              </div>
              <div class="col-6 p-relative">
                <div class="planet2 img-style">
                  <img src="@/assets/img/section8Img5.png" alt="" />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionEight",
  props: {},
};
</script>
<style lang="scss" scoped>
// style: color
.heading {
  font-size: 20px;
  &.s1 {
    color: #2ce2b7;
  }
  &.s2 {
    color: #f96deb;
  }
  &.s3 {
    color: #00e0ff;
  }
  &.s4 {
    color: #806df9;
  }
}
.content-heading {
  color: white;
  font-size: 16px;
}
.box-s1 {
  box-shadow: 0 0 2px #6df9b5, 0 0 10px #6df9b5, 0 0;
  border-radius: 20px;
  min-height: 120px;
  position: relative;
  &::before {
    position: absolute;
    content: ("");
    width: 80px;
    height: 1px;
    background: #2ce2b7;
    top: 50%;
    right: 102%;
    border: 3px solid #2ce2b7;
    filter: blur(3.5px);
  }
  &::after {
    position: absolute;
    content: ("");
    width: 1px;
    height: 560px;
    background: #5d6cf1;
    top: 0%;
    right: 140%;
    border: 3px solid #061fff;
    filter: blur(3.5px);
  }
}
.box-s2 {
  box-shadow: 0 0 2px #f96deb, 0 0 10px #f96deb, 0 0 20px #f96deb;
  border-radius: 20px;
  min-height: 120px;
  position: relative;
  &::before {
    position: absolute;
    content: ("");
    width: 80px;
    height: 1px;
    background: #f96deb;
    top: 50%;
    right: 102%;
    border: 3px solid #f96deb;
    filter: blur(3.5px);
  }
}
.box-s3 {
  box-shadow: 0 0 2px #00e0ff, 0 0 10px #00e0ff, 0 0 20px #00e0ff;
  border-radius: 20px;
  min-height: 120px;
  position: relative;
  &::before {
    position: absolute;
    content: ("");
    width: 80px;
    height: 1px;
    background: #00e0ff;
    top: 50%;
    right: 102%;
    border: 3px solid #00e0ff;
    filter: blur(3.5px);
  }
}
.box-s4 {
  box-shadow: 0 0 2px #806df9, 0 0 10px #806df9, 0 0 20px #806df9;
  border-radius: 20px;
  min-height: 120px;
  position: relative;
  &::before {
    position: absolute;
    content: ("");
    width: 80px;
    height: 1px;
    background: #806df9;
    top: 50%;
    right: 102%;
    border: 3px solid #806df9;
    filter: blur(3.5px);
  }
}
.padding {
  padding-top: 500px;
  @media (max-width: 991px) {
    padding-top: 300px;
  }
}
.text {
  color: white;
  font-size: clamp(12px, 3.5vw, 20px);
}
.sub-text {
  color: white;
  font-size: 20px;
  @media (max-width: 991px) {
    font-size: 18px;
  }
}
.section8 {
  background-image: url("@/assets/img/background7.png");
  background-repeat: no-repeat;
  background-size: cover;
  height: 140vh;
  @media (max-width: 991px) {
    height: auto;
  }
  @media (max-width: 576px) {
    height: auto;
  }
  .des-one {
    &::before {
      position: absolute;
      top: 0;
      left: 0%;
      content: ("");
      width: 1px;
      height: 160px;
      border: 3px solid #ffffff;
      filter: blur(3px);
      margin-left: 20px;
    }
    &::after {
      position: absolute;
      top: 160px;
      left: 0%;
      content: url("@/assets/img/point.png");
    }
  }
  .title {
    font-size: clamp(12px, 3.5vw, 40px);
    text-shadow: 0 0 7px #061fff, 0 0 10px #061fff, 0 0 21px #061fff,
      0 0 42px #061fff, 0 0 82px #061fff;
    @media (max-width: 767px) {
      font-size: 30px;
      padding-left: 50px;
    }
  }
  .title-image {
    width: 100%;
    img {
      width: 100%;
      object-fit: scale-down;
    }
  }

  .p-relative {
    position: relative;
    .planet1 {
      position: absolute;
      top: 180%;
      left: 40%;
      max-width: 100%;
      img {
        width: 100%;
      }
      @media (max-width: 991px) {
        top: 250%;
      }
      &::before {
        position: absolute;
        content: ("");
        top: 50%;
        left: 110%;
        height: 1px;
        width: 160%;
        background-color: #03ccfe;
        border: 3px solid #03ccfe;
        filter: blur(3.5px);
        @media (max-width: 991px) {
          width: 140%;
          top: 53%;
        }
      }
      &::after {
        position: absolute;
        content: url("@/assets/img/right.png");
        top: 36%;
        left: 260%;
        @media (max-width: 991px) {
          left: 230%;
        }
      }
    }
    .galaxy {
      max-width: 100%;
      position: absolute;
      top: 100%;
      right: 10%;
      img {
        width: 120%;
      }
      &::before {
        position: absolute;
        content: ("");
        top: 110px;
        left: 120%;
        height: 1px;
        width: 51%;
        background-color: #03ccfe;
        border: 3px solid #03ccfe;
        filter: blur(3.5px);
        @media (max-width: 991px) {
          top: 80px;
          width: 54%;
        }
      }
    }
    .cup {
      width: 100%;
      position: absolute;
      top: -100%;
      left: 20%;
      img {
        width: 60%;
      }
      @media (max-width: 991px) {
        top: -40%;
      }
      &::before {
        position: absolute;
        content: ("");
        top: 60px;
        left: 90%;
        height: 1px;
        width: 200%;
        background-color: #03ccfe;
        border: 3px solid #03ccfe;
        filter: blur(3.5px);
      }
      &::after {
        position: absolute;
        content: url("@/assets/img/left.png");
        top: 38px;
        right: 10%;
      }
    }
    .planet2 {
      width: 100%;
      position: absolute;
      top: -160px;
      left: 0%;
      img {
        width: 100%;
      }
      @media (max-width: 991px) {
        top: -100px;
      }
      &::before {
        position: absolute;
        top: -230px;
        left: 44%;
        content: ("");
        width: 1px;
        height: 210px;
        border: 4px solid #03ccfe;
        filter: blur(3px);
        margin-left: 20px;
        @media (max-width: 991px) {
          top: -120px;
          height: 100px;
        }
      }
      &::after {
        position: absolute;
        top: -30px;
        left: 44%;
        content: url("@/assets/img/down.png");
        @media (max-width: 991px) {
          top: -40px;
        }
      }
    }
  }
}
</style>

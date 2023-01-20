<template>
  <div id="container-test">
    <div class="bg-why">
      <img src="@/assets/img/section5Img1.png" alt="" class="logo" />
    </div>

    <div class="item box-1" :class="{ active: contentActive === 1 }">
      <div class="icon-des">
        <img src="@/assets/img/section5Img2.png" alt="" class="icon" />
        <p>Play game earn token</p>
      </div>
    </div>

    <div class="item box-2" :class="{ active: contentActive === 2 }">
      <div class="icon-des">
        <img src="@/assets/img/section5Img3.png" alt="" class="icon" />
        <p>Profits</p>
      </div>
    </div>

    <div class="item box-3" :class="{ active: contentActive === 3 }">
      <div class="icon-des">
        <img src="@/assets/img/section5Img4.png" alt="" class="icon" />
        <p>Upgrade NFT</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SpinView",
  data() {
    return {
      contentActive: null,
      timeOut: null,
      windowWidth: 1000,
    };
  },
  mounted() {
    this.onWindowResize();
  },
  destroyed() {
    window.removeEventListener("resize", this.onWindowResize);
  },
  methods: {
    activeSome() {
      if (this.contentActive == null || this.contentActive > 3) {
        this.contentActive = 1;
      }
      this.timeOut = setTimeout(() => {
        this.contentActive += 1;
        this.activeSome();
      }, 2000);
    },
    onWindowResize() {
      this.windowWidth = window.innerWidth;
      if (this.windowWidth <= 768) {
        clearTimeout(this.timeOut);
        this.activeSome();
      } else if (this.timeOut != null) {
        clearTimeout(this.timeOut);
      }
    },
  },
};
</script>

<style lang="scss" scoped>
#container-test {
  --n: 3; /* number of item */
  --d: 25s; /* duration */
  position: relative;
  max-width: 650px;
  width: 100%;
  height: 650px;
  margin: 0 auto;
  display: grid;
  place-content: center;
  border-radius: 50%;
  @media (max-width: 1200px) {
    width: 600px;
    height: 550px;
  }
  @media (max-width: 991px) {
    width: 500px;
    height: 500px;
  }
  @media (max-width: 575px) {
    width: 100%;
    height: 350px;
  }
  .bg-why {
    img {
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      margin: auto;
      z-index: 0;
    }
    .logo {
      max-width: 280px;
      width: 100%;
      height: 300px;
      @media (max-width: 1200px) {
        max-width: 260px;
        height: 268px;
      }
      @media (max-width: 991px) {
        max-width: 175px;
        height: 186px;
      }
      @media (max-width: 575px) {
        max-width: 100px;
        height: 115px;
      }
    }
  }
}
@keyframes rote2 {
  0% {
    transform: rotate(360deg);
  }
  100% {
    transform: rotate(0deg);
  }
}
.box-1 {
  background: linear-gradient(
    149.06deg,
    #3d64c9 12.21%,
    rgba(129, 156, 255, 0.62) 86.33%
  );
  box-shadow: 0 0 2px rgb(61, 100, 201, 0.12), 0 0 10px rgb(61, 100, 201, 0.12),
    0 0 20px rgba(129, 156, 255, 0.62), 0 0 30px rgba(129, 156, 255, 0.62),
    0 0 40px rgba(129, 156, 255, 0.62), 0 0 50px rgba(129, 156, 255, 0.62);
}
.box-2 {
  background: linear-gradient(
    149.06deg,
    #c93d3d 12.21%,
    rgba(255, 129, 129, 0.62) 86.33%
  );
  box-shadow: 0 0 2px rgba(255, 131, 131, 0.12),
    0 0 10px rgba(255, 131, 131, 0.12), 0 0 20px rgba(255, 129, 129, 0.62),
    0 0 30px rgba(255, 129, 129, 0.62), 0 0 40px rgba(255, 129, 129, 0.62),
    0 0 50px rgba(255, 129, 129, 0.62);
  transform: rotate(0deg);
  .icons {
    transform: rotate(0deg);
  }
}

.box-3 {
  background: linear-gradient(
    149.06deg,
    #a43dc9 12.21%,
    rgba(255, 129, 227, 0.62) 86.33%
  );
  box-shadow: 0 0 2px rgba(164, 61, 201, 0.12),
    0 0 10px rgba(164, 61, 201, 0.12), 0 0 20px rgba(255, 129, 227, 0.62),
    0 0 30px rgba(255, 129, 227, 0.62), 0 0 40px rgba(255, 129, 227, 0.62),
    0 0 50px rgba(255, 129, 227, 0.62);
  transform: rotate(2deg);
  .icons {
    transform: rotate(-2deg);
  }
}
.item {
  width: 115px;
  height: 115px;
  display: flex;
  position: relative;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  z-index: 20;
  border-radius: 100%;
  .icon-des {
    position: absolute;
    top: 18%;
    left: 50%;
    transform: translate(-50%, -18%);
    width: 65px;
    height: 65px;
    z-index: 10;
    @media (max-width: 991px) {
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
    }
    img {
      width: 100%;
      height: 100%;
      object-fit: scale-down;
      @media (max-width: 991px) {
        width: 50px;
        height: 50px;
      }
      @media (max-width: 575px) {
        width: 30px;
        height: 30px;
      }
    }
    p {
      font-family: "Poppins";
      font-style: normal;
      font-weight: 500;
      font-size: clamp(8px, 1.5vw, 10px);
      line-height: 130%;
      text-align: center;
      letter-spacing: 0.1em;

      color: #ffffff;
    }
  }
  // animation: rote2 20s infinite linear;
  @media (max-width: 991px) {
    width: 100px;
    height: 100px;
  }
  @media (max-width: 575px) {
    width: 70px;
    height: 70px;
  }
  .bg {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    width: 100%;
    height: 100%;
    z-index: 1;
  }
}
.item {
  grid-area: 1/1;
  line-height: 30px;
  // background: #f00;
  animation: spin var(--d) linear infinite;
  transform: rotate(0) translate(255px) rotate(0);
  @media (max-width: 1200px) {
    animation: spinTablet var(--d) linear infinite;
    transform: rotate(0) translate(185px) rotate(0);
  }
  @media (max-width: 575px) {
    animation: spinMb var(--d) linear infinite;
    transform: rotate(0) translate(115px) rotate(0);
  }
}
@keyframes spin {
  100% {
    transform: rotate(1turn) translate(255px) rotate(-1turn);
  }
}
@keyframes spinTablet {
  100% {
    transform: rotate(1turn) translate(185px) rotate(-1turn);
  }
}
@keyframes spinMb {
  100% {
    transform: rotate(1turn) translate(115px) rotate(-1turn);
  }
}
.item:nth-child(1) {
  animation-delay: calc(-0 * var(--d) / var(--n));
}
.item:nth-child(2) {
  animation-delay: calc(-1 * var(--d) / var(--n));
}
.item:nth-child(3) {
  animation-delay: calc(-2 * var(--d) / var(--n));
}
/*.item:nth-child(N) {animation-delay:calc(-(N - 1)*var(--d)/var(--n))}*/
</style>

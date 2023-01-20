<template>
  <div class="section1">
    <div class="header">
      <b-navbar toggleable="lg" type="dark" variant="info">
        <b-navbar-brand href="#"
          ><img class="img-size" src="@/assets/img/logo.png"
        /></b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item
              class="text"
              v-for="(item, idx) in headerItems"
              :key="item + idx"
            >
              <router-link :to="item.href">
                {{ item.title }}
              </router-link>
            </b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
    <div class="content">
      <div class="item1">HERO SNAKE</div>
      <div class="item2">Keep fun - Earn money</div>
      <div class="section1-img" data-aos="zoom-in">
        <img src="@/assets/img/img1.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyBaner",
  props: {},
  data() {
    return {
      headerItems: [
        {
          id: 1,
          title: "Home",
          href: "/home",
        },
        {
          id: 2,
          title: "Token HBG",
          href: "/road-map",
        },
        {
          id: 3,
          title: "Ecosytem",
          href: "#section3",
        },
        {
          id: 4,
          title: "Document",
          href: "#section4",
        },
        {
          id: 5,
          title: "Marketplace",
          href: "#section5",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.section1 {
  // max-width: 1920px;
  // max-height: 1122px;
  width: 100%;
  height: 100vh;
  background-image: url("@/assets/img/background1.png");
  background-repeat: no-repeat;
  background-size: cover;
  .header {
    .img-size {
      @media (max-width: 1400px) {
        max-width: 170px;
        max-height: 80px;
        margin-left: 60px;
      }
      @media (max-width: 991px) {
        max-width: 180px;
        margin-left: 20px;
      }
      @media (max-width: 661px) {
        max-width: 100px;
        max-height: 60px;
        margin-left: 0px;
      }
    }
  }
  .content {
    position: absolute;
    top: 28%;
    left: 50%;
    transform: translateX(-50%);
    max-width: 390px;
    max-height: 380px;
    color: white;
    font-weight: 600;
    background: rgba(255, 255, 255, 0.1);
    border: 1px solid rgba(255, 255, 255, 0.5);
    border-radius: 10px;
    padding: 20px;
    @media (max-width: 661px) {
      // width: 60%;
      // height: 40%;
      padding: 10px;
    }
    .item1 {
      padding: 10px 0;
      font-size: 20px;
    }
    .item2 {
      margin-bottom: 40px;
    }
    .section1-img {
      width: 100%;
      img {
        width: 100%;
        border-radius: 8px;
        object-fit: scale-down;
      }
    }
  }

  //   @media (max-width: 991px);
  // }

  .navbar-dark .navbar-nav .nav-link {
    color: rgb(247, 240, 240);
    font-weight: 600;
    font-size: 24px;
    @media (max-width: 341px) {
      font-size: 16 px;
    }
  }
  .navbar-toggler {
    @media (max-width: 991px) {
      font-size: 2.5rem;
    }
    @media (max-width: 661px) {
      font-size: 2rem;
    }
    @media (max-width: 480px) {
      font-size: 1.3rem;
    }
  }
  ul.navbar-nav {
    width: 100%;
    display: flex;
    justify-content: space-evenly;
  }
  .bg-info {
    background-color: rgba(136, 134, 134, 0.1) !important;
    @media (max-width: 991px) {
      background-color: #000c37 !important;
      z-index: 10;
      .text {
        text-align: left;
      }
    }
  }
}
</style>

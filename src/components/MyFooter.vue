<template>
  <div class="footer py-4 container-fluid">
    <div class="wrap-footer row">
      <div class="col-lg-6 col-12" data-aos="fade-right">
        <div class="col-lg-2 col-12 logo">
          <img src="@/assets/img/logo.png" />
        </div>
        <div class="tag">
          <div class="c1">HOME</div>
          <div class="c1">TOKEN HBG</div>
          <div class="c1">HEROCOIN</div>
          <div class="c1">MARKETPLACE</div>
          <div class="c1">DOCUMENT</div>
        </div>
      </div>
      <div class="contact col-md-12 col-lg-6">
        <div class="item1" data-aos="fade-up">Contact with us</div>

        <form data-aos="fade-left">
          <div class="form-group">
            <input
              type="text"
              class="form-control"
              id="exampleInputEmail1"
              aria-describedby="emailHelp"
              placeholder="Email"
            />
            <input
              type="text"
              class="form-control custom-style"
              id="exampleInputEmail1"
              aria-describedby="emailHelp"
              placeholder="Details of your inquiry"
            />
          </div>
        </form>
        <div class="btn" data-aos="fade-left">
          <button class="btn-item">SEND</button>
        </div>
        <div class="item3" data-aos="fade-up">
          <div class="custom-size">CẬP NHẬT THÔNG TIN TẠI ĐÂY:</div>
          <div class="icon">
            <img class="icon1" src="@/assets/img/youtube.svg" alt="" />
            <img class="icon2" src="@/assets/img/tele.svg" alt="" />
            <img class="icon3" src="@/assets/img/fb.svg" alt="" />
            <img class="icon4" src="@/assets/img/tw.svg" alt="" />
            <img class="icon5" src="@/assets/img/discord.svg" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyFooter",
  props: {},
};
</script>
<style lang="scss" scoped>
.logo {
  width: 100%;
  text-align: left;
  img {
    width: 100%;
    object-fit: scale-down;
    @media (max-width: 991px) {
      width: 30%;
    }
  }
}
.footer {
  background-image: url("@/assets/img/background8.png");
  background-repeat: no-repeat;
  background-size: cover;
  min-height: 100vh;
  width: 100%;
  .form-group > input {
    color: #fff;
    font-size: auto;
  }
  .form-group > input {
    width: 78%;
    height: 100px;
    margin: 10px 0;
    background: rgba(255, 255, 255, 0.1);
    @media (max-width: 991px) {
      width: 100%;
    }
    @media (max-width: 662px) {
      width: 100%;
      height: 60px;
    }
  }
  .form-group > input::placeholder {
    color: rgb(189, 185, 185);
    font-weight: 600;
    @media (max-width: 991px) {
      font-size: 30px;
    }
    @media (max-width: 661px) {
      font-size: 16px;
    }
  }
  .tag {
    color: #fff;
    font-size: 30px;
    text-align: left;
    font-style: italic;
    margin: 40px 40px;
    @media (max-width: 661px) {
      font-size: 20px;
      margin: 10px 20px;
    }
  }
  .wrap-footer {
    position: relative;
    display: flex;
    height: 100%;
    .wrap-content {
      margin-top: 20vh;
      padding-left: 20px;
      flex: 1;
      @media (max-width: 991px) {
        margin-top: 6vh;
      }
      @media (max-width: 662px) {
        margin-top: 6vh;
      }

      .content {
        display: flex;
        margin: 10px 0;
        .content1 {
          width: 60%;
          text-align: left;
          color: #fff;
          @media (max-width: 991px) {
            font-size: 20px;
          }
          @media (max-width: 661px) {
            font-size: 12px;
          }
        }
      }
    }
    .contact {
      flex: 1;
      padding: 20px;
      .item1 {
        margin-top: 10%;
        text-align: left;
        color: #fff;
        font-size: 20px;
        @media (max-width: 991px) {
          font-size: 40px;
          margin-top: 10px;
          padding-left: 20px;
        }
        @media (max-width: 661px) {
          font-size: 24px;
          margin-top: 10px;
          padding-left: 20px;
        }
      }
      .item3 > div:first-of-type {
        color: #fff;
        font-size: 20px;
        text-align: left;
        @media (max-width: 991px) {
          font-size: 30px;
        }
        @media (max-width: 661px) {
          font-size: 18px;
        }
      }
      .item3 {
        padding-top: 60px;
        .icon > img {
          margin: 10px 20px;
          width: 30px;
          height: 30px;
          @media (max-width: 991px) {
            width: 60px;
            height: 60px;
          }
          @media (max-width: 661px) {
            width: 30px;
            height: 30px;
            margin: 10px 8px;
          }
        }
        .icon {
          text-align: left;
          @media (max-width: 991px) {
            text-align: center;
          }
        }
      }

      .item2 {
        margin-top: 30px;
        padding: 20px 10px;
        text-align: left;
        width: 80%;
        color: #000;
        background-color: #ececec;
        @media (max-width: 991px) {
          width: 100%;
          margin-top: 10px;
          padding: 20px 20px;
          font-size: 20px;
        }
      }
      .item2 > div {
        padding: 6px 0;
        font-weight: 500;
      }
      .btn {
        width: 80%;
        margin-right: 20%;
        text-align: right;
        @media (max-width: 991px) {
          margin-right: -24px;
          width: 100%;
        }

        .btn-item {
          min-width: 160px;
          min-height: 60px;
          border-radius: 8px;
          background: linear-gradient(
            180deg,
            rgba(0, 255, 163, 0.7) 0%,
            rgba(83, 218, 193, 0.553) 100%
          );
          box-shadow: 3px 2px 6px rgba(22, 216, 99, 0.37);
          border-radius: 37px;
          font-size: 24px;
          color: white;
          @media (max-width: 991px) {
            min-width: 200px;
            min-height: 60px;
            font-size: 30px;
          }
          @media (max-width: 661px) {
            min-width: 80px;
            min-height: 40px;
            font-size: 16px;
          }
        }
      }
    }
  }
}
</style>

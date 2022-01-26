<template>
  <div class="container content">
    <div class="image">
      <img src="../../assets/cup2.png" alt="" />
    </div>
    <div class="content-text">
      <div class="row">
        <div class="col-md-6">
          <div class="text-head">
            <h2 class="h1" id="title">
              Dark <br />
              Coffee
            </h2>
            <bottom class="btn" id="order-now">Order now</bottom>
          </div>
        </div>
        <div class="col-md-6">
          <div class="text">
            <div class="wave-p" id="wave">
              <img src="../../assets/Shape.png" alt="" id="image" />
              <p class="info" id="info">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum
                dolor at itaque, temporibus debitis exercitationem. Illo non
                enim nihil sit, esse ipsa ullam ratione obcaecati qui unde
                possimus voluptas aut. Lorem ipsum dolor sit amet consectetur
                adipisicing elit. Veniam odit animi facere delectus aut? Fugiat,
                tempore ex facilis vero alias adipisci id hic molestias,
                blanditiis, laudantium nulla? Labore, odio sunt!
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "DarkCoffe",
};
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
.content {
  height: 100vh;
  .image {
    position: relative;
    img {
      position: absolute;
      width: 25%;
      top: 50%;
      left: 50%;
      transform: translate(-50%);
      padding-top: 15%;
      z-index: 99;
    }
  }
  .content-text {
    position: relative;
    .text-head {
      h2 {
        @extend .coffee-font;
        font-size: 130px !important;
        padding-top: 140px;
        padding-bottom: 90px;
      }
      bottom {
        @extend .order-now-bottom;
      }
    }
    .text {
      position: relative;
      .wave-p {
        position: absolute;
        top: 0px;
        left: 16px;
        width: 120%;
        height: 100vh;
        img {
          width: 107%;
          position: absolute;
          top: -2px;
          left: -53px;
          height: 102%;
        }
        p {
          position: absolute;
          top: 30%;
          left: 20%;
          right: 10%;
          color: #fff;
          line-height: 1.8;
          font-size: 19px;
          font-weight: 600;
        }
      }
    }
  }
}

// Medium devices (tablets, 768px and up)
// @media only screen and (max-width: 600px > < 960px) {
@media (min-width: 600px) and (max-width: 960px) {
  #wave {
    margin-top: 0;
  }
}
@media (max-width: 1096px) {
  #title {
    padding-top: 100px;
  }

  .image img {
    display: none;
  }
  #wave {
    background-color: $color-blue;
    left: 0;
    height: 60vh;
    width: 100%;
    margin-top: 100px;

    #image {
      display: none;
    }
    #info {
      top: 30px;
      left: 15px;
      right: 15px;
      padding-top: 0;
    }
  }
  .text-head {
    h2 {
      text-align: center;
      font-size: 95px;
      padding-top: 10px;
      padding-bottom: 35px;
    }
    .text-head bottom {
      margin-bottom: 30px;
    }
  }
  #order-now {
    margin-bottom: 25px;
  }
}

// Small devices (landscape phones, 576px and up)
// @media (min-width: 576px) and (max-width: 991.98px) {
//   #title {
//     padding-top: 100px;
//   }

//   .image img {
//     display: none;
//   }
//   #wave {
//     background-color: $color-blue;
//     left: 0;
//     height: 70vh;
//     width: 100%;

//     #image {
//       display: none;
//     }
//     #info {
//       top: 30px;
//       left: 15px;
//       right: 15px;
//       padding-top: 0;
//     }
//   }
//   .text-head {
//     h2 {
//       text-align: center;
//       font-size: 95px;
//       padding-top: 10px;
//       padding-bottom: 35px;
//     }
//     .text-head bottom {
//       margin-bottom: 30px;
//     }
//   }
//   #order-now {
//     margin-bottom: 25px;
//   }
// }
// Large devices (desktops, 992px and up)
// @media (min-width: 992px) {
//   #wave {
//     margin-top: 100px;
//     #info {
//       padding-top: 0;
//     }
//   }
// }
</style>

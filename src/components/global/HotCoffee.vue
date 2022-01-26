<template>
  <div class="container content" id="content">
    <div class="image">
      <img src="../../assets/hot-coffee.png" alt="" />
    </div>
    <div class="content-text">
      <div class="row">
        <div class="col-md-6">
          <div class="text-head">
            <h2 class="h1" id="title">
              Hot <br />
              Coffee
            </h2>
            <bottom class="btn" id="order-now">Order now</bottom>
          </div>
        </div>
        <div class="col-md-6">
          <div class="text">
            <div class="wave-p" id="wave">
              <img src="../../assets/Shape-3.png" alt="" id="image" />
              <p id="info">
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
  name: "HotCoffe",
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
        // position: absolute;
        // top: 0px;
        // left: 16px;
        // width: 120%;
        // height: 100vh;
        // background: url("../../assets/Shape-3.png") no-repeat;
        position: absolute;
        top: 0px;
        left: 16px;
        width: 120%;
        height: 100vh;
        img {
          position: absolute;
          width: 107%;
          top: -6px;
          left: -53px;
          height: 101%;
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

@media (min-width: 600px) and (max-width: 960px) {
  #content {
    margin-top: 81vh;
  }
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
    height: 70vh;
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
</style>

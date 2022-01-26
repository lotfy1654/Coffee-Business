<template>
  <div class="info">
    <div class="container">
      <div class="gift">
        <div class="row">
          <div class="col-md-6 col-sm">
            <div class="content text-center">
              <img src="../../assets/coffee-bean.png" alt="" />
              <h2 class="h1">Free</h2>
            </div>
          </div>
          <div class="col-md-6 col-sm">
            <div class="gift-text text-center">
              <h2 class="h1 text-capitalize">gift voucher</h2>
              <h3 class="text-capitalize">1 cup of coffee</h3>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Ullam
                velit ipsum autem, ipsa facilis animi minima natus illo aliquam!
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
.info {
  border: 3px solid $color-blue;
  .gift {
    margin: 60px 0;
    padding: 50px;
    border: 8px solid $color-blue;
    .content {
      background-color: $color-blue;
      border-radius: 50%;
      border: 5px solid $color-red;
      color: #fff;
      width: 300px;
      height: 300px;
      margin: 0px 115px;
      img {
        width: 80px;
        padding-top: 40px;
      }
      h2 {
        font-size: 70px;
        font-weight: bold;
      }
    }
    .gift-text {
      h2 {
        @extend .coffee-font;
        font-size: 80px !important;
      }
      h3 {
        background-color: rgba(255, 74, 0, 0.57);
        border: 3px solid $color-red;
        border-radius: 10px;
        width: 250px;
        margin: 30px 0 30px 160px;
        padding: 10px;
      }
      p {
        font-size: 16px;
        font-weight: 500;
        color: $color-blue;
      }
    }
  }
}
</style>

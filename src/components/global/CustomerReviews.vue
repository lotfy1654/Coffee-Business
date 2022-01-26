<template>
  <div class="container">
    <div class="client">
      <h2 class="h1 text-center">Customer Reviews</h2>
      <div class="review">
        <div class="row">
          <div class="col-md-6">
            <img src="../../assets/customer.png" alt="" />
          </div>
          <div class="col-md-6">
            <div class="box text-center">
              <h2 class="h1">john peter</h2>
              <p>
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ea
                hic, ad recusandae omnis aperiam suscipit voluptate iure
                debitis. Nulla reiciendis ut nesciunt. Facilis quos recusandae
                aliquid, exercitationem nam vero sequi?
              </p>
            </div>
            <div class="box text-center">
              <h2 class="h1">ella thomson</h2>
              <p>
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ea
                hic, ad recusandae omnis aperiam suscipit voluptate iure
                debitis. Nulla reiciendis ut nesciunt. Facilis quos recusandae
                aliquid, exercitationem nam vero sequi?
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="open text-center">
        <h2>We are open</h2>
        <div class="time-box">
          <h3>Monday - Friday</h3>
          <h3>8:00 am - 11:30 pm</h3>
        </div>
        <div class="time-box">
          <h3>Sarturday - Sunday</h3>
          <h3>9:00 am - 10:30 pm</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
.client {
  .h1 {
    @extend .coffee-font;
    font-style: normal;
    font-size: 75px;
    padding: 30px 0;
    font-family: Cormorant Garamond;
    font-weight: 600;
  }
  .review {
    background-color: $color-blue;
    padding: 30px;
    .box {
      color: #fff;
      margin: 80px 0;
      .h1 {
        color: #fff;
        text-transform: capitalize;
        font-size: 50px;
      }
      p {
        font-size: 15px;
        padding: 0 35px;
      }
    }
  }
  .open {
    margin-top: 100px;
    h2 {
      color: $color-blue;
      font-family: Cormorant Garamond;
      font-weight: 600;
      font-size: 65px;
    }
    .time-box {
      background-color: $color-blue;
      margin: 70px 30%;
      padding: 30px;
      color: #fff;
      box-shadow: 4px 3px 8px $color-blue;
    }
  }
}
</style>

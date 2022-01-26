<template>
  <div class="header">
    <div class="image"></div>
    <div class="container">
      <div class="nav">
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
          <div class="container-fluid">
            <button
              class="navbar-toggler"
              type="button"
              data-bs-toggle="collapse"
              data-bs-target="#navbarNavAltMarkup"
              aria-controls="navbarNavAltMarkup"
              aria-expanded="false"
              aria-label="Toggle navigation"
            >
              <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
              <div class="navbar-nav">
                <a class="nav-link" aria-current="page" href="#">Home</a>
                <a class="nav-link" href="#">About</a>
                <a class="nav-link" href="#">Menu</a>
                <a class="nav-link" href="#">Blog</a>
                <a class="nav-link" href="#">Shop</a>
                <a class="nav-link" href="#">Contact</a>
              </div>
            </div>
          </div>
        </nav>
      </div>
      <div class="header-text">
        <h2>Coffee</h2>
        <p>Everything you love about Coffee</p>
        <p class="info">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto,
          animi fuga. Magnam harum aliquam aut aspernatur fuga rerum.
        </p>
        <div class="order-now">
          <bottom class="btn">Order now</bottom>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss">
@import "../../assets/style/variables.scss";

.header {
  position: relative;
  .image {
    background-image: url("../../assets/header.png");
    background-size: cover;
    width: 100%;
    height: 100vh;
  }
  .nav {
    padding: 40px 0 0 0;
    position: absolute;
    top: 0;
    .bg-light {
      background: none !important;
    }
    a {
      &.active {
        border-bottom: 5px solid $color-red;
      }
      color: $color-blue !important;
      font-size: 25px;
      margin-right: 20px;
      &:hover {
        border-bottom: 5px solid $color-red;
      }
    }
  }
  .header-text {
    position: absolute;
    top: 20%;
    padding: 20px 0 0 0;
    h2 {
      @extend .coffee-font;
    }
    p:first-of-type {
      color: $color-red;
      font-size: 25px;
      font-weight: bold;
      padding-top: 10px;
      text-transform: capitalize;
    }
    .info {
      width: 40%;
      font-size: 20px;
      font-weight: 400;
    }
    .order-now {
      padding-top: 20px;
      bottom {
        @extend .order-now-bottom;
      }
    }
  }
}

@media screen and (max-width: 576px) {
  .header .image {
    background: none;
    height: 90vh;
  }
  .header-text h2 {
    font-size: 100px;
    text-align: center;
  }
  .header .header-text p:first-of-type {
    text-align: center;
  }
  .header .header-text .info {
    width: auto;
    text-align: center;
  }
}
</style>

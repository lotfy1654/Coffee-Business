<template>
  <div class="container">
    <h2 class="text-center">Our pranches</h2>
    <div class="card-group">
      <div class="card">
        <img src="../../assets/new-york.png" class="card-img-top" alt="..." />
        <div class="card-body">
          <h5 class="card-title text-capitalize">new york</h5>
          <p class="card-text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor
            inventore blanditiis placeat fugit odit hic nihil accusantium
            sapiente totam laudantium ut perferendis voluptate, corporis
            excepturi quam quasi? Tempore, qui libero!
          </p>
        </div>
      </div>
      <div class="card">
        <img src="../../assets/texas.png" class="card-img-top" alt="..." />
        <div class="card-body">
          <h5 class="card-title text-capitalize">texas</h5>
          <p class="card-text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor
            inventore blanditiis placeat fugit odit hic nihil accusantium
            sapiente totam laudantium ut perferendis voluptate, corporis
            excepturi quam quasi? Tempore, qui libero!
          </p>
        </div>
      </div>
      <div class="card">
        <img src="../../assets/new-jersy.png" class="card-img-top" alt="..." />
        <div class="card-body">
          <h5 class="card-title text-capitalize">new jersy</h5>
          <p class="card-text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor
            inventore blanditiis placeat fugit odit hic nihil accusantium
            sapiente totam laudantium ut perferendis voluptate, corporis
            excepturi quam quasi? Tempore, qui libero!
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
.container {
  h2 {
    color: $color-blue;
    text-transform: capitalize;
    font-size: 55px;
    padding: 30px 0;
    font-weight: 600;
  }
}
.card-group {
  margin-bottom: 70px;
  .card {
    background-color: #233e6a;
    color: #fff;
    margin: 20px;
    padding: 5px;
    .card-body {
      position: relative;
      .card-title {
        background-color: $color-red;
        width: 120px;
        position: absolute;
        padding: 10px;
        border-radius: 10px;
        top: -25px;
        left: -15px;
      }
      .card-text {
        background-color: $color-blue;
        padding: 30px;
        margin-top: 15px;
      }
    }
  }
}
</style>

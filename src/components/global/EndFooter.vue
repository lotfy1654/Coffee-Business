<template>
  <div class="footer">
    <div class="container">
      <div class="row">
        <div class="col-md-6 text-start">
          <div class="footer-image">
            <img src="../../assets/coffee-bean.png" alt="" />
            <h2>CoffeeCup</h2>
          </div>
        </div>
        <div class="col-md-3 nav-footer">
          <h2>Information.</h2>
          <ul>
            <li><a href="#">About</a></li>
            <li><a href="#">Menu</a></li>
            <li><a href="#">Blog</a></li>
            <li><a href="#">Shop</a></li>
          </ul>
        </div>
        <div class="col-md-3 contact">
          <h2>Contact</h2>
          <ul>
            <li>Support</li>
            <li>lotfy1654@gmail.com</li>
          </ul>
        </div>
      </div>
    </div>
    <footer>
      <p class="text-center">Create with love by Lotfy mohamed</p>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";
.footer {
  background-image: linear-gradient(to bottom right, $color-blue, #233e6a);
  color: #fff;
  padding-top: 60px;
  .footer-image {
    img {
      width: 50px;
    }
    h2 {
      display: inline-block;
    }
  }
  .nav-footer {
    ul {
      list-style: none;
      li {
        a {
          color: #fff;
          text-decoration: none;
          &:hover {
            color: $color-red;
          }
        }
      }
    }
  }
  .contact {
    ul {
      list-style: none;
      li {
        &:hover:last-child {
          color: $color-red;
          cursor: pointer;
        }
      }
    }
  }
  footer {
    background-color: #233e6a;
    padding: 10px;
    p {
      font-size: 18px;
      margin: 2px;
      font-weight: 500;
      text-transform: capitalize;
    }
  }
}
</style>

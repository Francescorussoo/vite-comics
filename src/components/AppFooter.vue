<template>
  <footer class="footer-section">
    <div class="footer-links">
      <div class="footer-item">
        <img src="../../img/buy-comics-digital-comics.png" alt="Digital Comics">
        <a href="#">Digital Comics</a>
      </div>
      <div class="footer-item">
        <img src="../../img/buy-comics-merchandise.png" alt="DC Merchandise">
        <a href="#">DC Merchandise</a>
      </div>
      <div class="footer-item">
        <img src="../../img/buy-comics-subscriptions.png" alt="Subscription">
        <a href="#">Subscription</a>
      </div>
      <div class="footer-item">
        <img src="../../img/buy-comics-shop-locator.png" alt="Comic Shop Locator">
        <a href="#">Comic Shop Locator</a>
      </div>
      <div class="footer-item">
        <img src="../../img/buy-dc-power-visa.svg" alt="DC Power Visa">
        <a href="#">DC Power Visa</a>
      </div>
    </div>
    <div class="footer-info">
      <div class="info-column">
        <h4>DC Comics</h4>
        <ul>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">News</a></li>
        </ul>
        <h4>Shop</h4>
        <ul>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
        </ul>
      </div>
      <div class="info-column">
        <h4>DC</h4>
        <ul>
          <li><a href="#">Terms of Use</a></li>
          <li><a href="#">Privacy Policy</a></li>
          <li><a href="#">Ad Choices</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">News</a></li>
        </ul>
      </div>
      <div class="info-column">
        <h4>Sites</h4>
        <ul>
          <li><a href="#">MAD Magazine</a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC PowerVisa</a></li>
        </ul>
      </div>
      <img src="../../img/dc-logo-bg.png" alt="DC Logo" class="footer-logo">
    </div>
    <div class="footer-bottom">
      <div class="signup-section">
        <button class="signup-btn">SIGN UP NOW</button>
        <div class="social-section">
          <h5>FOLLOW US</h5>
          <div class="social-icons">
            <a href="#"><img src="../../img/footer-facebook.png" alt="Facebook"></a>
            <a href="#"><img src="../../img/footer-twitter.png" alt="Twitter"></a>
            <a href="#"><img src="../../img/footer-youtube.png" alt="YouTube"></a>
            <a href="#"><img src="../../img/footer-pinterest.png" alt="Pinterest"></a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'AppFooter'
}
</script>

<style lang="scss" scoped>
$footer-bg: #000;
$footer-text: #fff;
$link-hover: #0074e8;

.footer-section {
  background-color: $footer-bg;
  color: $footer-text;
  background-image: url(../../img/footer-bg.jpg);

  .footer-links {
    display: flex;
    justify-content: center;
    background-color: $link-hover;
    padding: 1.25rem 0;

    .footer-item {
      margin: 0 2.5rem;
      text-align: center;

      a {
        display: block;
        color: $footer-text;
        text-decoration: none;
        font-weight: bold;
        margin-top: 0.5rem;
        transition: color 0.3s;

        &:hover {
          color: lighten($link-hover, 15%);
        }
      }
    }
  }

  .footer-info {
    max-width: 75rem;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    padding: 1.25rem;

    .info-column {
      padding: 1.25rem;
      
      h4 {
        margin-bottom: 0.625rem;
        color: $footer-text;
      }

      ul {
        list-style: none;
        padding: 0;

        li {
          margin-bottom: 0.3125rem;

          a {
            color: $footer-text;
            text-decoration: none;
            font-size: 0.875rem;
            transition: text-decoration 0.3s;

            &:hover {
              text-decoration: underline;
            }
          }
        }
      }
    }

    .footer-logo {
      width: 100%;
      height: auto;
      margin-top: 1rem;
    }
  }

  .footer-bottom {
    background-color: darken($footer-bg, 5%);
    padding: 1.25rem 0;

    .signup-section {
      max-width: 62.5rem;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;

      .signup-btn {
        background: $footer-bg;
        color: $footer-text;
        border: 2px solid $link-hover;
        padding: 0.625rem;
        cursor: pointer;
        transition: all 0.3s;

        &:hover {
          background: $link-hover;
          color: $footer-bg;
        }
      }

      .social-section {
        text-align: center;

        h5 {
          margin-bottom: 0.625rem;
        }

        .social-icons {
          display: flex;
          gap: 0.5rem;
          justify-content: center;

          a {
            display: inline-block;
            transition: transform 0.3s;

            &:hover {
              transform: scale(1.1);
            }

            img {
              width: 1.5rem;
            }
          }
        }
      }
    }
  }
}
</style>

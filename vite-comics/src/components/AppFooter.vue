<script>
export default {

}

</script>

<template>
  <footer>
    <div class="calltoaction">
      <div class="container">
        <ul class="menu-calltoaction">
          <li class="item_calltoaction">
            <img src="/img/buy-comics-digital-comics.png" alt="">
            <p>DIGITAL COMICS</p>
          </li>
          <li class="item_calltoaction">
            <img src="/img/buy-comics-merchandise.png" alt="">
            <p>DC MERCHANDISE</p>
          </li>
          <li class="item_calltoaction">
            <img src="/img/buy-comics-subscriptions.png" alt="">
            <p>SUBSCRIPTION</p>
          </li>
          <li class="item_calltoaction">
            <img src="/img/buy-comics-shop-locator.png" alt="">
            <p>COMIC SHOP LOCATOR</p>
          </li>
          <li class="item_calltoaction">
            <img src="/img/buy-dc-power-visa.svg" alt="">
            <p>DC POWER VISA</p>
          </li>
        </ul>
      </div>
    </div>
    <div class="menu-link">
      <div class="container">
        <div class="row">
          <div class="list">
            <ul class="list_link">
              <li>DC COMICS</li>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movies</li>
              <li>TV</li>
              <li>Games</li>
              <li>Videos</li>
              <li>News</li>
            </ul>
            <ul class="list_link">
              <li>DC</li>
              <li>Terms Of Use</li>
              <li>Privacy policy (New)</li>
              <li>Ad Choices</li>
              <li>Advertising</li>
              <li>Jobs</li>
              <li>Subscription</li>
              <li>Talent Workshops</li>
              <li>CPSC Certificates</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contact Us</li>
            </ul>
            <ul class="list_link">
              <li>SITES</li>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
            <ul class="list_link">
              <li>SHOP</li>
              <li>Shop DC</li>
              <li>Shop DC Collactibles</li>
            </ul>
          </div>
          <div class="logo">
            <img src="/img/dc-logo-bg.png" alt="">
          </div>
        </div>
      </div>
    </div>
    <div class="community">
      <div class="container">
        <div class="row row-space">
          <div class="community_signup">
            <div class="signup">
              <a href="#">
                <p>SIGN-UP NOW!</p>
              </a>
            </div>
          </div>
          <div class="community_social">
            <ul class="social">
              <li>FOLLOW US</li>
              <li>
                <a href="#">
                  <img src="/img/footer-facebook.png" alt="">
                </a>
              </li>
              <li>
                <a href="#">
                  <img src="/img/footer-periscope.png" alt="">
                </a>
              </li>
              <li>
                <a href="#">
                  <img src="/img/footer-pinterest.png" alt="">
                </a>
              </li>
              <li>
                <a href="#">
                  <img src="/img/footer-twitter.png" alt="">
                </a>
              </li>
              <li>
                <a href="#">
                  <img src="/img/footer-youtube.png" alt="">
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use '../style/partials/variable' as *;
@use '../style/general.scss' as *;


.menu-calltoaction {
  display: flex;
  align-items: center;
  margin: 0px 15px;
}

.item_calltoaction {
  flex-basis: calc(100%*(8/12));
  display: flex;
  align-items: center;
  justify-content: space-around;

  & img {
    width: 40px;
  }

  & p {
    flex-grow: 1;
    margin-left: 10px;
    font-size: 12px;
    color: white;
  }
}

.calltoaction {
  padding: 40px;
  background-color: $color-active-link;
}

.menu-link {
  background-image: url('/img/footer-bg.jpg');

  & li {
    color: #959595;
  }

  .list_link li:first-child {
    color: white;
  }

  .logo {
    flex-basis: calc(100%*(5/12));
    text-align: right;
  }

  .list {
    flex-basis: calc(100%*(3/12));
    display: flex
  }
}

.community {
  background-color: #303030;
  padding: 40px;

  .row-space {
    justify-content: space-between;
  }

  .social li:first-child {
    color: $color-active-link;
  }

  .social {
    display: flex;
    align-items: center;
    gap: 15px;
  }

  .signup {
    color: white;
    border: 3px solid $color-active-link;
    padding: 15px;
  }
}
</style>
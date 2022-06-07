<template>
  <div class="finish">
    <div class="container">
      <div class="finish-wrapper">
        <div class="finish-wrapper__text">
          <div class="finish-info">
            <div class="finish-info__item">
              <div class="finish-info__image">
                <img src="@/assets/img/United.png" alt="" />
              </div>
              <div class="finish-info__title">
                9470 192 St. Surrey, BC <br />Canada V4N 3R9
              </div>
              <button class="finish-btn">contact us</button>
            </div>
          </div>
          <div class="finish-block">
            <div class="finish-info__body">
              <div class="finish-body__title">Free Yourself</div>
              <div class="finish-body__subtitle">
                <p>Skin care</p>
                <p>Shower & Bath</p>
                <p>Bundles</p>
                <p>Clothing</p>
              </div>
            </div>
            <div class="finish-info__body">
              <div class="finish-body__title">Company</div>
              <div class="finish-body__subtitle">
                <p>About</p>
                <p>Our Products</p>
                <p>30 Day love It</p>
                <p>FAQs</p>
                <p>Sitemap</p>
              </div>
            </div>
            <div class="finish-info__body">
              <div class="finish-body__title">Follow Us</div>
              <div class="finish-body__subtitle">
                <p>Facebook</p>
                <p>Twitter</p>
                <p>Instagram</p>
                <p>Free Life Blog</p>
              </div>
            </div>
          </div>
        </div>
        <div class="finish-text">
          <div class="finish-text__title">
            Copyright © 2020 United and Free. All Rights Reserved.
          </div>
          <div class="finish-text__body">
            <div class="finish-text__subtitle">Accepted Payments</div>
            <div class="finish-text__image">
              <img src="@/assets/img/finish.svg" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Finish",
};
</script>

<style lang="scss" scoped>
.finish {
  padding: 50px 0;
}
.finish-wrapper__text {
  display: flex;
  justify-content: space-between;
}
.finish-info__image {
  width: 100%;
  padding-bottom: 30px;
}
.finish-info__title {
  color: #6d6d6d;
  padding-bottom: 30px;
}
.finish-btn {
  background: black;
  color: white;
  border-radius: 3px;
  cursor: pointer;
  padding: 15px 60px;
}
.finish-btn:active {
  color: black;
  background: white;
  font-size: 20px;
}
.finish-block {
  display: flex;
  gap: 100px;
}
.finish-body__title {
  font-size: 27px;
  padding-bottom: 30px;
}
.finish-body__subtitle p {
  color: #6d6d6d;
  padding-bottom: 15px;
}
.finish-text {
  display: flex;
  justify-content: space-between;
  margin-top: 50px;
  align-items: center;
}
.finish-text__body {
  display: flex;
  gap: 40px;
  align-items: center;
}
.finish-text__image img {
  width: 100%;
}
.finish-text__title {
  color: #6d6d6d;
  font-size: 15px;
  align-items: center;
}
.finish-text__subtitle {
  color: #6d6d6d;
  font-size: 15px;
}
@media screen and (max-width: 992px) {
  .finish-wrapper__text {
    display: flex;
    flex-direction: column;
  }
  .finish-block {
    display: flex;
    justify-content: center;
  }
  .finish-info {
    display: flex;
    justify-content: center;
    margin-bottom: 30px;
  }
}
@media screen and (max-width: 768px) {
  .finish-text__body {
    gap: 10px;
  }
}
@media screen and (max-width: 576px) {
  .finish-block {
    display: flex;
    flex-direction: column;
    text-align: center;
  }
  .finish-text {
    display: flex;
    flex-direction: column;
    margin-top: 30px;
    gap: 15px;
  }
  .finish-info {
    display: flex;
    justify-content: center;
    margin-bottom: 30px;
    text-align: center;
  }
  .finish-block {
    gap: 30px;
  }
  .finish-text__title {
    font-size: 12px;
  }
}
</style>

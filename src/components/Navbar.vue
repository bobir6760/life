<template>
  <div class="navbar">
    <div class="container">
      <div class="navbar-wrapper">
        <div class="navbar-info">
          <div class="navbar-wrapper__image">
            <img src="@/assets/img/FREE.png" alt="" />
          </div>
          <div class="navbar-wrapper__item">
            <div class="navbar__item">About</div>
            <div class="navbar__subtitle">products</div>
          </div>
          <div class="navbar-wrapper__text">
            <div class="navbar-text__title">log in</div>
            <div class="navbar-text__subtitle">cart</div>
            <div class="navbar__text">usd</div>
          </div>
        </div>
        <div class="navbar-body">
          <div class="navbar-body__title">Hassle Free Personal Care</div>
          <div class="navbar-body__subtitle">
            Quality hair and skincare products for men and women delivered to
            your door
          </div>
          <button class="navbar-btn">buy now</button>
        </div>

        <div class="navbar-block">
          <div class="navbar-block__image">
            <img src="@/assets/img/Scarlett.png" alt="" />
          </div>
          <div class="navbar-block__item">
            <div class="navbar-block__title">
              I don’t wear makeup very often, but when I do I go for a
              natural,<br />
              no-makeup look. This skin tint and concealer gives exactly
              that.<br />
              It helps even out my skin tone and looks very natural.
            </div>
            <div class="navbar-block__subtitle">- Scarlett Black</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style lang="scss" scoped>
.navbar {
  padding: 50px 0px;
  background-image: url("~@/assets/img/home1.png");
  background-size: cover;
}
.navbar-info {
  display: flex;
  justify-content: space-between;
}
.navbar-wrapper__image img {
  width: 100%;
}
.navbar-wrapper__item {
  display: flex;
  gap: 40px;
  color: white;
  font-size: 20px;
}
.navbar-wrapper__text {
  display: flex;
  gap: 40px;
  color: white;
}
.navbar-body {
  text-align: center;
  margin-top: 100px;
}
.navbar-body__title {
  color: white;
  font-size: 95px;
  margin-bottom: 20px;
}
.navbar-body__subtitle {
  font-size: 20px;
  color: white;
  margin-bottom: 40px;
}
.navbar-btn {
  padding: 20px 45px;
  font-size: 20px;
  cursor: pointer;
  margin-bottom: 50px;
  border-radius: 3px;
  border: none;
}
.navbar-btn:active {
  font-size: 25px;
  background-color: black;
  color: white;
}
.navbar-block {
  display: flex;
  gap: 63px;
  background-color: white;
}
.navbar-block__title {
  font-size: 20px;
}
.navbar-block__subtitle {
  color: red;
  font-size: 20px;
}
.navbar-block__item {
  padding-top: 64px;
}
.navbar-block__image img {
  width: 100%;
}
@media screen and (max-width: 992px) {
  .navbar-body__title {
    font-size: 50px;
  }
  .navbar-block__item {
    padding-top: 45px;
  }
  .navbar-block {
    display: flex;
    gap: 20px;
  }
  .navbar-block__title {
    padding-bottom: 24px;
  }
}
@media screen and (max-width: 768px) {
  .navbar-info {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 40px;
  }
  .navbar-body__title {
    font-size: 40px;
  }
  .navbar-body__subtitle {
    font-size: 15px;
  }
  .navbar-btn {
    font-size: 15px;
    padding: 15px 35px;
  }
  .navbar-block__item {
    padding: 20px 0px;
  }
  .navbar-block {
    display: flex;
    gap: 20px;
    background-color: white;
  }
  .navbar-block__title {
    font-size: 15px;
    margin-bottom: 15px;
  }
}
@media screen and (max-width: 576px) {
  .navbar-block {
    display: flex;
    flex-direction: column;
  }
  .navbar-block__item {
    padding: 0px 5px;
  }
}
</style>

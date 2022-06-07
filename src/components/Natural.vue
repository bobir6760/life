<template>
  <div class="natural">
    <div class="container">
      <div class="natural-wrapper">
        <div class="natural-info">
          <div class="natural-info__title">
            We don’t just care about hair & skin. <br />we care about you.
          </div>
        </div>
        <div class="natural-block">
          <div class="natural-block__image">
            <img src="@/assets/img/Scarlett.png" alt="" />
          </div>
          <div class="natural-block__item">
            <div class="natural-block__title">
              I don’t wear makeup very often, but when I do I go for a
              natural,<br />
              no-makeup look. This skin tint and concealer gives exactly
              that.<br />
              It helps even out my skin tone and looks very natural.
            </div>
            <div class="natural-block__subtitle">- Scarlett Black</div>
          </div>
        </div>
        <div class="natural-block">
          <div class="natural-block__image">
            <img src="@/assets/img/Scarlett.png" alt="" />
          </div>
          <div class="natural-block__item">
            <div class="natural-block__title">
              I don’t wear makeup very often, but when I do I go for a
              natural,<br />
              no-makeup look. This skin tint and concealer gives exactly
              that.<br />
              It helps even out my skin tone and looks very natural.
            </div>
            <div class="natural-block__subtitle">- Scarlett Black</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Natural",
};
</script>

<style lang="scss" scoped>
.natural {
  padding: 50px 0px;
}
.natural-wrapper {
  background: #f7f7f7;
  padding: 10px;
}
.natural-info__title {
  font-size: 30px;
  text-transform: uppercase;
  text-align: center;
  margin-bottom: 30px;
}
.natural-block {
  display: flex;
  justify-content: center;
  gap: 80px;
  margin-bottom: 20px;
}
.natural-block__image img {
  width: 100%;
}
.natural-block__title {
  font-size: 12px;
  padding-top: 10%;
}
.natural-block__subtitle {
  color: red;
  font-size: 25px;
  padding-top: 20px;
  cursor: pointer;
}
.natural-block__subtitle:active {
  color: black;
}
.natural-block__item {
  align-items: flex-end;
}
@media screen and (max-width: 992px) {
  .natural-info__title {
    font-size: 20px;
    text-align: center;
  }
  .natural-block {
    display: flex;
    gap: 30px;
    margin-bottom: 30px;
  }
}
@media screen and (max-width: 768px) {
  .natural-block__item {
    text-align: center;
  }
  .natural-info__title {
    font-size: 17px;
    text-transform: uppercase;
    text-align: center;
    margin-bottom: 30px;
  }
  .natural-block__subtitle {
    color: red;
    font-size: 20px;
    padding-top: 20px;
  }
  .natural-block {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin-bottom: 30px;
  }
}
@media screen and (max-width: 576px) {
  .natural-block {
    display: flex;
    flex-direction: column;
  }
  .natural-block__title {
    padding: 0px;
    font-size: 20px;
    text-align: center;
  }
  .natural-block__subtitle {
    color: red;
    font-size: 17px;
    padding-top: 20px;
    text-align: center;
  }
  .natural-block__image img {
    width: 100%;
  }
}
</style>

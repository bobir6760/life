<template>
  <div class="absolut">
    <div class="container">
      <div class="absolut-wrapper">
        <div class="absolut-info">
          <div class="absolut-title">
            why united and free is the effortless choice
          </div>
        </div>
        <div class="absolut-item">
          <div class="absolut-wrapper-item">
            <div class="absolut-text">
              <div class="absolut-text__title">
                Direct delivery to your door.
              </div>
              <div class="absolut-text__subtitle">
                Order your products from the comfort of <br />your home
              </div>
            </div>
            <div class="absolut-text">
              <div class="absolut-text__title">
                Safe for all skin+hair types
              </div>
              <div class="absolut-text__subtitle">
                PH balanced and small batch tested
              </div>
            </div>
            <div class="absolut-text">
              <div class="absolut-text__title">Made for man and women</div>
              <div class="absolut-text__subtitle">
                Everyone can enjoy the product line
              </div>
            </div>
          </div>
          <div class="absolut-wrapper__image">
            <div class="absolut-image">
              <img src="@/assets/img/ABSOLUT.png" alt="" />
            </div>
          </div>
          <div class="absolut-block">
            <div class="absolut-wrapper__text">
              <div class="absolut-block__title">Leaping bunny certified</div>
              <div class="absolut-block__subtitle">
                All products are plant besed and cruelty free
              </div>
            </div>
            <div class="absolut-wrapper__text">
              <div class="absolut-block__title">Leaping bunny certified</div>
              <div class="absolut-block__subtitle">
                All products are plant besed and cruelty free
              </div>
            </div>
          </div>
        </div>
        <div class="absolute-button">
          <button class="absolut-btn">buy now</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Absolut",
};
</script>

<style lang="scss" scoped>
.absolut {
  padding: 50px 0px;
}
.absolut-item {
  display: flex;
}
.absolut-title {
  font-size: 40px;
  text-align: center;
  margin-bottom: 100px;
  cursor: pointer;

}
.absolut-text {
  display: flex;
  flex-direction: column;
  gap: 15px;
}
.absolut-text__subtitle {
  margin-bottom: 80px;
  cursor: pointer;

}
.absolut-text__title {
  font-size: 25px;
  cursor: pointer;

  font-weight: bold;
}
.absolute-text__title {
  font-size: 25px;
  font-weight: bold;
  cursor: pointer;

}
.absolut-block {
  display: flex;
  flex-direction: column;
}
.absolut-block__title {
  font-size: 25px;
  font-weight: bold;
  margin-bottom: 15px;
  cursor: pointer;

}
.absolut-block__subtitle {
  margin-bottom: 80px;
}
.absolut-image img {
  width: 100%;
  cursor: pointer;

}
.absolute-button {
  display: flex;
  justify-content: center;
}
.absolut-btn {
  padding: 15px 55px;
  font-size: 20px;
  color: white;
  background-color: black;
  cursor: pointer;
  border-radius: 5px;
  border: none;
}
.absolut-btn:hover {
  background-color: #971717;
  transition: 0.5s;
}
@media screen and (max-width: 768px) {
  .absolut-text__title {
    font-size: 15px;
  }
  .absolut-text__subtitle {
    margin-bottom: 30px;
    font-size: 13px;
  }
  .absolut-text {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  .absolut-block__title {
    font-size: 15px;
  }
  .absolut-block__subtitle {
    margin-bottom: 30px;
    font-size: 13px;
  }
  .absolut-title {
    font-size: 30px;
  }
  .absolut-btn {
    font-size: 15px;
    padding: 12px 25px;
  }
}
@media screen and (max-width: 576px) {
  .absolut-item {
    display: flex;
    flex-direction: column;
  }
  .absolut-wrapper-item {
    text-align: center;
  }
  .absolut-block {
    text-align: center;
  }
  .absolut-title {
    font-size: 30px;
    margin-bottom: 40px;
  }
  .absolut-btn {
    font-size: 11px;
    padding: 10px 22px;
  }
}
</style>

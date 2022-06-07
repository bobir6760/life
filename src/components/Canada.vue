<template>
  <div class="canada">
    <div class="container">
      <div class="canada-wrapper">
        <div class="canada-info">
          <div class="canada-info__title">as featured in</div>
        </div>
        <div class="canada-item">
          <div class="canada-item__image">
            <img src="@/assets/img/Group 17.png" alt="" />
          </div>
          <div class="canada-item__image">
            <img src="@/assets/img/Group 18.png" alt="" />
          </div>
          <div class="canada-item__image">
            <img src="@/assets/img/Group 19.png" alt="" />
          </div>
          <div class="canada-item__image">
            <img src="@/assets/img/Group 20.png" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Canada",
};
</script>

<style lang="scss" scoped>
.canada {
  padding: 50px 0px;
}
.canada-info__title {
  text-transform: uppercase;
  font-size: 30px;
  padding-bottom: 20px;
}
.canada-item {
  display: flex;
  justify-content: center;
  gap: 20px;
}
.canada-item__image img {
  width: 100%;
}
@media screen and (max-width: 992px) {
  .canada-info__title {
    text-align: center;
  }
}
@media screen and (max-width: 768px) {
  .canada-item {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
  }
}
@media screen and (max-width: 576px) {
  .canada-item {
    display: flex;
    flex-direction: column;
  }
  .canada-info__title {
    font-size: 25px;
  }
}
</style>

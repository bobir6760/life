<template>
  <div class="stop">
    <div class="container">
      <div class="stop-wrapper">
        <div class="stop-wrapper__image">
          <img src="@/assets/img/my home.png" alt="" />
        </div>
        <div class="stop-info">
          <div class="stop-info__title">
            Stop stressing out over buying your personal care products
          </div>
          <button class="stop-btn">buy now</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Stop",
};
</script>

<style lang="scss" scoped>
.stop {
  padding: 50px 0;
}
.stop-wrapper {
  display: flex;
  align-items: center;
  gap: 30px;
}
.stop-wrapper__image img {
  width: 100%;
}
.stop-info {
  background: #f7f7f7;
  padding: 40px;
}
.stop-btn {
  cursor: pointer;
  background: black;
  color: white;
  padding: 12px 50px;
  font-size: 15px;
  border-radius: 3px;
  border: none;
}
.stop-btn:active {
  color: black;
  background: white;
  font-size: 20px;
}
.stop-info__title {
  font-size: 20px;
  padding-bottom: 30px;
}
@media screen and (max-width: 768px) {
  .stop-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;
  }
  .stop-info {
    display: flex;
    flex-direction: column;
    text-align: center;
    align-items: center;
  }
}
@media screen and (max-width: 576px) {
  .stop-btn {
    padding: 10px 40px;
    font-size: 13px;
  }
}
</style>

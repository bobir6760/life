<template>
  <div class="with-card">
    <div class="with-item">
      <div class="with-item__image">
        <img :src="item.imgUrl" alt="" />
      </div>
      <div class="with-item__title">{{ item.title }}</div>
      <div class="with-item__subtitle">{{ item.subtitle }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "with-card",
  props: {
    item: {
      type: Object,
      require: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.with-card {
  display: flex;
  gap: 20px;
}
.with-item {
  text-align: start;
  background-color: white;
  padding: 30px;
}
.with-item__image img {
  margin-bottom: 10px;
  object-fit: contain;
  width: 70px;
  height: 70px;
}
.with-item__title {
  font-size: 22px;
  font-weight: bold;
  margin-bottom: 10px;
}
.with-item__subtitle {
  color: #6d6d6d;
  font-size: 15px;
}
@media screen and (max-width: 768px) {
  .with-info__title {
    font-size: 22px;
  }
  .with-block {
    gap: 5px;
  }
}
@media screen and (max-width: 576px) {
  .with-item {
    display: flex;
    flex-direction: column;
    gap: 15px;
  }
  .with-item {
    text-align: center;
  }
  .with-info__title {
    font-size: 25px;
  }
}
</style>

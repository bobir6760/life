<template>
  <div class="shop-wrapper__item">
    <div class="shop-wrapper__image">
      <div class="shop-image">
        <img :src="item.imgUrl" alt="" />
      </div>
      <div class="shop-title">{{ item.title }}</div>
      <div class="shop-subtitle">{{ item.subtitle }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "shop-card",
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped lang="scss">
.shop-wrapper__item {
  display: flex;
  gap: 60px;
}
.shop-image img {
  width: 100%;
  cursor: pointer;
}
.shop-title {
  font-size: 25px;
  padding: 20px 0;
  cursor: pointer;
}
.shop-subtitle {
  cursor: pointer;
}
</style>

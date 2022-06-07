<template>
  <div class="like-info">
    <div class="like-block">
      <div class="like-info__image">
        <img :src="item.imgUrl" alt="" />
      </div>
      <div class="like-info__title">{{ item.title }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "like-card",
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped lang="scss">
.like-info__title {
  font-size: 24px;
  color: #6d6d6d;
  margin-top: 20px;
}
.like-info__image {
  text-align: center;
}
.like-info__image img {
  object-fit: contain;
  width: 50px;
  height: 50px;
}
</style>

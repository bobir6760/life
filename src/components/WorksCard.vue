<template>
  <div class="works-item-wrapper">
    <div class="works-title">{{ item.title }}</div>
    <div class="works-info__subtitle">{{ item.subtitle }}</div>
  </div>
</template>

<script>
export default {
  name: "works-card",
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.works-item-wrapper {
  display: flex;
  flex-direction: column;
  gap: 15px;
  padding: 50px;
  background: #f7f7f7;
}
.works-info__subtitle {
  color: #6d6d6d;
  font-size: 18px;
  cursor: pointer;
}
.works-title {
  color: #c0335d;
  font-size: 30px;
  cursor: pointer;
}
.works-title:hover {
  text-decoration: underline crimson;
}
@media screen and (max-width: 768px) {
  .works-info__subtitle {
    display: flex;
    flex-direction: column;
  }
}
</style>

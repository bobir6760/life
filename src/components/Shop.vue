<template>
  <div class="shop">
    <div class="container">
      <div class="shop-wrapper">
        <div class="shop-info">
          <div class="shop-info__title">shop united & free</div>
        </div>
        <div class="shop-wrapper-card">
          <ShopCard v-for="(card, index) in cards" :key="index" :item="card" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ShopCard from "@/components/ShopCard";
export default {
  name: "Shop",
  data() {
    return {
      cards: [
        {
          imgUrl: require("@/assets/img/overlay.png"),
          title: "Absolut",
          subtitle: "face and Body Lotion",
        },
        {
          imgUrl: require("@/assets/img/overlay2.png"),
          title: "Absolut",
          subtitle: "face and Body Lotion",
        },
        {
          imgUrl: require("@/assets/img/overlay3.png"),
          title: "Absolut",
          subtitle: "face and Body Lotion",
        },
      ],
    };
  },
  components: {
    ShopCard,
  },
};
</script>

<style lang="scss" scoped>
.shop {
  padding: 50px 0;
  background: #f7f7f7;
}
.shop-info {
  text-align: center;
}
.shop-info__title {
  font-size: 40px;
  text-transform: uppercase;
  margin-bottom: 60px;
}
.shop-wrapper-card {
  display: flex;
  gap: 60px;
}
@media screen and (max-width: 768px) {
  .shop-info__title {
    font-size: 30px;
    margin-bottom: 30px;
  }
  .shop-title {
    padding: 10px 0;
    font-size: 20px;
  }
  .shop-subtitle {
    font-size: 15px;
  }
  .shop-wrapper__item {
    display: flex;
    gap: 10px;
  }
}
@media screen and (max-width: 576px) {
  .shop-wrapper__item {
    display: flex;
    flex-direction: column;
    gap: 50px;
  }
  .shop-title {
    padding: 10px 0;
    font-size: 25px;
  }
  .shop-subtitle {
    font-size: 20px;
  }
  .shop-info__title {
    font-size: 28px;
    margin-bottom: 20px;
  }
}
.shop-wrapper-card {
  flex-direction: column;
}
</style>

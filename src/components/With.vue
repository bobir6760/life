<template>
  <div class="with">
    <div class="container">
      <div class="with-wrapper">
        <div class="with-info">
          <div class="with-info__title">Do you struggle with</div>
          <div class="with-wrapper-card">
            <WithCard
              v-for="(card, index) in cards"
              :key="index"
              :item="card"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import WithCard from "@/components/WithCard";
export default {
  name: "With",
  data() {
    return {
      cards: [
        {
          imgUrl: require("@/assets/img/icn1.svg"),
          title: "Bathroom Clutter",
          subtitle: "Too many products for everyone in your household",
        },
        {
          imgUrl: require("@/assets/img/icn2.svg"),
          title: "Dry Skin",
          subtitle:
            "Caused by seasonal changes,allergies, excessive hand washing",
        },
        {
          imgUrl: require("@/assets/img/icn3.svg"),
          title: "Damaged Hair",
          subtitle: "Dry, split ends, brittle, or color damaged",
        },
      ],
    };
  },
  components: {
    WithCard,
  },
};
</script>

<style lang="scss" scoped>
.with {
  padding: 50px 0px;
  background-color: #f7f7f7;
}
.with-info {
  display: flex;
  flex-direction: column;
  gap: 30px;
}
.with-info__title {
  font-size: 30px;
  cursor: pointer;
}
.with-wrapper-card {
  display: flex;
  flex-direction: column;
  gap: 20px;
}
@media screen and (max-width: 992px) {
  .with-info__title {
    padding: 0px;
  }
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
  .with-block {
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
  .with-wrapper-card {
    flex-direction: column;
  }
}
</style>

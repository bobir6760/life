<template>
  <div class="like">
    <div class="container">
      <div class="like-wrapper">
        <div class="like-wrapper__title">Just like you we care about</div>
        <div class="like-wrapper-card">
          <LikeCard v-for="(card, index) in cards" :key="index" :item="card" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import LikeCard from "@/components/LikeCard";
export default {
  name: "Like",
  data() {
    return {
      cards: [
        {
          imgUrl: require("@/assets/img/art1.svg"),
          title: "Cruelty Free Products",
        },
        {
          imgUrl: require("@/assets/img/art1.svg"),
          title: "Cruelty Free Products",
        },
        {
          imgUrl: require("@/assets/img/art1.svg"),
          title: "Cruelty Free Products",
        },
        {
          imgUrl: require("@/assets/img/art1.svg"),
          title: "Cruelty Free Products",
        },
      ],
    };
  },
  components: {
    LikeCard,
  },
};
</script>

<style lang="scss" scoped>
.like {
  padding: 50px 0;
}
.like-wrapper__title {
  font-size: 37px;
  text-align: center;
  text-transform: uppercase;
  margin-bottom: 60px;
  cursor: pointer;
}
.like-wrapper__title:hover {
  text-decoration: underline crimson;
}
.like-wrapper-card {
  display: flex;
  gap: 50px;
  justify-content: center;
  text-align: center;
}
@media screen and (max-width: 992px) {
  .like-info {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
  }
  .like-info__title {
    font-size: 20px;
    text-align: center;
    margin-bottom: 40px;
  }
  .like-wrapper__title {
    font-size: 33px;
    margin-bottom: 40px;
  }
}
@media screen and (max-width: 768px) {
  .like-wrapper__title {
    font-size: 25px;
    margin-bottom: 35px;
  }
}
@media screen and (max-width: 576px) {
  .like-info {
    display: flex;
    flex-direction: column;
  }
  .like-info__title {
    margin-top: 10px;
  }
  .like-wrapper-card {
    flex-direction: column;
  }
}
</style>

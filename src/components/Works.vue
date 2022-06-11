<template>
  <div class="works">
    <div class="container">
      <div class="works-wrapper">
        <div class="works-title">How it works</div>
        <div class="works-card-wrapper">
          <WorksCard v-for="(card, index) in cards" :key="index" :item="card" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import WorksCard from "@/components/WorksCard";

export default {
  name: "Works",
  components: { WorksCard },
  data() {
    return {
      cards: [
        {
          title: "01",
          subtitle: "Order online from the comfort of your home",
        },
        {
          title: "02",
          subtitle: "Order online from the comfort of your home",
        },
        {
          title: "03",
          subtitle: "Order online from the comfort of your home",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.works {
  padding: 50px 0;
}
.works-title {
  text-align: center;
  font-size: 30px;
  text-transform: uppercase;
  margin-bottom: 50px;
  cursor: pointer;
}
.works-title:hover {
  text-decoration: underline crimson;
  transition: 0.5s;
}
.works-card-wrapper {
  display: flex;
  justify-content: center;
  gap: 50px;
}
@media screen and (max-width: 576px) {
  .works-card-wrapper {
    flex-direction: column;
  }
}
</style>

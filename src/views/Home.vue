<template>
  <div class="home">
    <Navbar />
    <With />
    <Absolut />
    <Natural />
    <Canada />
    <Shop />
    <Like />
    <Works />
    <Stop />
    <Finish />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import With from "@/components/With.vue";
import Absolut from "@/components/Absolut.vue";
import Natural from "@/components/Natural.vue";
import Canada from "@/components/Canada.vue";
import Shop from "@/components/Shop.vue";
import Like from "@/components/Like.vue";
import Works from "@/components/Works.vue";
import Stop from "@/components/Stop.vue";
import Finish from "@/components/Finish.vue";
export default {
  name: "Home",
  components: {
    Navbar,
    With,
    Absolut,
    Natural,
    Canada,
    Shop,
    Like,
    Works,
    Stop,
    Finish,
  },
};
</script>

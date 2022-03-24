<template>
  <div class="box">
    <div class="head"><Header /></div>
    <div class="foot"><Footer /></div>
    <div><router-view></router-view></div>
  </div>
</template>

<script>
import Header from "@/pages/header.vue";
import Footer from "@/pages/footer.vue";

export default {
  components: { Header, Footer },
};
</script>

<style scoped>
.box {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
</style>

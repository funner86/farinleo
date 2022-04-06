<template>
  <div class="box">
    <Header class="head" />
    <div class="news"><News /></div>
    <div class="Virtual">虚拟展厅</div>
    <div class="exhibit"><Chenlie /></div>
    <div class="activity"><Activity /></div>
    <div class="foot"><Footer /></div>
    <div><router-view></router-view></div>
  </div>
</template>

<script>
import Header from "@/pages/header.vue";
import Footer from "@/pages/footer.vue";
import News from "@/pages/news.vue";
import Chenlie from "@/pages/chenlie";
import Activity from "@/pages/activity";

export default {
  components: { Header, Footer, News, Chenlie, Activity },
};
</script>

<style scoped>
.box {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
</style>

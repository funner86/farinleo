<template>
  <div class="big">
    <div class="show"></div>
    <div class="footer">
      <oj>
        <li><img src="@/images/ZD_03.png" alt="" @click="change" /></li>
        <li><img src="" alt="" @click="change" /></li>
        <li></li>
        <li></li>
        <li></li>
      </oj>
    </div>
  </div>
</template>

<script>
import Test from "@/lib/Test.vue";
import Test from "../lib/Test.vue";
export default {
  components: { TestTest },
  data() {
    return {
      sendUrl: "",
    };
  },
  methods: {
    change(e) {
      thi.sendUrl = context;
    },
  },
};
</script>

<style>
</style>
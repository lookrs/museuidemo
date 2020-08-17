<template>
  <div class="home">
    <Topbar></Topbar>
    <NavTop></NavTop>
  </div>
</template>

<script>
import NavTop from "@/components/NavTop.vue";
import Topbar from "@/components/Topbar.vue";

export default {
  name: "Home",
  components: {
    NavTop,
    Topbar,
  },
  
};
</script>
<style>
.demo-list-wrap {
  width: 100%;
  max-width: 100%;
  overflow: hidden;
}
</style>
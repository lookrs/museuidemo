<template>
  <div class="descr">
    <mu-container v-if="isShow">
      <mu-card style="width: 100%; max-width: 375px; margin: 0 auto;">
        <mu-card-title title="温馨提示"></mu-card-title>
        <mu-card-text>
          1、班干可见字段，收集信息时可直接获取并导出表格
          2、记得及时维护更新自己的信息，以及设置班干要收集的信息为可见
        </mu-card-text>
        <mu-card-actions>
          <mu-button flat v-on:click="controll">知道啦</mu-button>
        </mu-card-actions>
      </mu-card>
    </mu-container>
  </div>
</template>

<script>
export default {
  name: "Descr",
  data() {
    return {
      isShow: true,
    };
  },
  methods: {
    controll() {
      this.isShow = !this.isShow;
    },
  }
};
</script>

<style scoped>
.descr{
    margin-top: 10px;
}
</style>
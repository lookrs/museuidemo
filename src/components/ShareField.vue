<template>
  <div class="ShareField">
   <mu-container  class="demo-chip-wrapper">
  <mu-chip class="demo-chip" v-for="chip,index in chips" :key="chip" :color="chipscolor[index%7]" @delete="remove(index)" delete>{{chip}}</mu-chip>
  <mu-button color="primary" v-if="chips.length === 0" @click="reset">载入基本信息</mu-button>
</mu-container>
  </div>
</template>

<script>
export default {
  name: 'ShareFiled',
  data () {
    return {
      chipscolor:['primary', 'secondary', 'success', 'warning', 'info', 'error',""],
      chips: ['primary', 'secondary', 'success', 'warning', 'info', 'error', '姓名', '性别', '年龄'],

    }
  },
  methods: {
    remove (index) {
      this.chips.splice(index, 1);
    },
    reset () {
      this.chips = ['primary', 'secondary', 'success', 'warning', 'info', 'error'];
    }
  }
}
</script>

<style scoped>
.demo-chip-wrapper {
  text-align: center;
}
.demo-chip {
  margin: 8px;
  vertical-align: middle;
}
.ShareField {
  overflow: auto;
  max-height: 380px;
}
</style>
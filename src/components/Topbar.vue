<template>
  <div class="topbar">
   <mu-paper :z-depth="1" class="demo-list-wrap">
      <mu-appbar color="pink">
        <mu-menu slot="left">
          <mu-button flat>
            <mu-icon value="menu"></mu-icon>
          </mu-button>
          <mu-list slot="content">
            <mu-list-item button>
              <mu-list-item-content>
                <mu-list-item-title>当前用户</mu-list-item-title>
              </mu-list-item-content>
            </mu-list-item>
            <mu-divider></mu-divider>
            <mu-list-item button>
              <mu-list-item-content>
                <mu-list-item-title>修改密码</mu-list-item-title>
              </mu-list-item-content>
            </mu-list-item>
            <mu-divider></mu-divider>
            <mu-list-item button>
              <mu-list-item-content>
                <mu-list-item-title>退出账号</mu-list-item-title>
              </mu-list-item-content>
            </mu-list-item>
            <mu-divider></mu-divider>
            <mu-list-item button>
              <mu-list-item-content>
                <mu-list-item-title>关于</mu-list-item-title>
              </mu-list-item-content>
            </mu-list-item>
          </mu-list>
        </mu-menu>我的信息列表{{changeTitle}}
        <mu-button icon slot="right" @click="addField">
          <mu-icon value="add" ></mu-icon>
        </mu-button>
      </mu-appbar>
    </mu-paper>
  </div>
</template>

<script>
export default {
  name: "Topbar",
  data(){
     return{
       changeTitle: "1",
       barName: "新建"
     } 
  },
  methods:{
    addField(){
      this.$router.push("/FieldEdit")
      this.$state.topTitle=this.barName
    },
    
  },
  mounted:{
    changeTitle(){
      this.changeTitle = this.$state.topTitle
    }
  }
}
</script>

<style scoped>

</style>
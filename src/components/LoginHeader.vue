<template>
  <div class="loginheader">
    <mu-appbar style="width: 100%;" color="primary">
      <!-- <mu-button icon slot="left">
        <mu-icon value="menu"></mu-icon>
      </mu-button> -->
      登录
      <mu-menu slot="right">
        <!-- <mu-button flat>菜单</mu-button>
        <mu-list slot="content">
          <mu-list-item button>
            <mu-list-item-content>
              <mu-list-item-title>关于</mu-list-item-title>
            </mu-list-item-content>
          </mu-list-item>
          <mu-list-item button>
            <mu-list-item-content>
              <mu-list-item-title>说明</mu-list-item-title>
            </mu-list-item-content>
          </mu-list-item>
        </mu-list> -->
      </mu-menu>
    </mu-appbar>
  </div>
</template>

<script>
export default {
  name: "LoginHeader",
};
</script>

<style scoped>
</style>

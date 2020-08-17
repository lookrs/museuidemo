<template>
  <div class="Left-up">
    <mu-menu slot="left">
      <mu-button flat>
        <mu-icon value="menu"></mu-icon>
      </mu-button>
      <mu-list slot="content">
        <mu-list-item button>
          <mu-list-item-content>
            <mu-list-item-title>关于</mu-list-item-title>
          </mu-list-item-content>
        </mu-list-item>
        <mu-list-item button>
          <mu-list-item-content>
            <mu-list-item-title>信息</mu-list-item-title>
          </mu-list-item-content>
        </mu-list-item>
      </mu-list>
    </mu-menu>
  </div>
</template>

<script>
export default {
  name: "Left-up",
};
</script>

<style scoped>
</style>
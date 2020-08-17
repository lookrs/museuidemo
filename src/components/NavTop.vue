<template>
  <div class="NavTop">
    <mu-tabs :value.sync="active2" color="green" indicator-color="yellow" full-width>
      <mu-tab>班干可见</mu-tab>
      <mu-tab>所有字段</mu-tab>
    </mu-tabs>
    <div class="demo-text" v-if="active2 === 0">
      <ShareField></ShareField>
      
    </div>
    <div class="demo-text" v-if="active2 === 1">
     <InfoList></InfoList> 
    </div>  
    <Descr></Descr>
  </div>
</template>

<script>
import InfoList from "@/components/InfoList.vue";
import ShareField from "@/components/ShareField.vue";
import Descr from "@/components/Desc.vue";
export default {
  name: "NavTop",
  components: {
    InfoList,
    ShareField,
    Descr
  },
  data() {
    return {
      active2: 0,
    };
  },
};
</script>

<style >
.demo-text {
  padding: 16px;
  background: #fff;
}
p {
  margin: 8px 0;
}
.NavTop{
    margin-top: 10px;
}
</style>
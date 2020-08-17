<template>
  <div class="FieldEdit">
    <Topbar></Topbar>
    <mu-container>
      <mu-form :model="form" class="mu-demo-form" :label-position="labelPosition" label-width="100">
        <mu-form-item prop="input" label="信息字段名">
          <mu-text-field v-model="form.inputField"></mu-text-field>
        </mu-form-item>
        <mu-form-item prop="input" label="字段值">
          <mu-text-field v-model="form.inputFieldValue"></mu-text-field>
        </mu-form-item>
      </mu-form>
    </mu-container>
  </div>
</template>

<script>
import Topbar from "@/components/Topbar.vue";
export default {
  name: "FieldEdit",
  components:{
Topbar ,
  },
  data() {
    return {
      labelPosition: 'right',
      form: {
        inputField: "",
        inputFieldValue: "",
        
      },
    };
  },
};
</script>

<style scoped>
.mu-demo-form {
  width: 100%;
  max-width: 460px;
}
</style>
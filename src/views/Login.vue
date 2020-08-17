<template>
  <div class="login">
    
    <LoginHeader></LoginHeader>
    <mu-container>
      <mu-paper class="demo-paper mpaper" :z-depth="5">
        <mu-form ref="form" :model="validateForm" class="mu-demo-form">
          <mu-form-item label="用户名" help-text="3-10位" prop="username" :rules="usernameRules">
            <mu-text-field v-model="validateForm.username" prop="username"></mu-text-field>
          </mu-form-item>
          <mu-form-item label="密码" prop="password" :rules="passwordRules">
            <mu-text-field type="password" v-model="validateForm.password" prop="password"></mu-text-field>
          </mu-form-item>
          <mu-form-item prop="isAgree" :rules="argeeRules">
            <mu-checkbox label="同意用户协议" v-model="validateForm.isAgree"></mu-checkbox>
          </mu-form-item>
          <mu-form-item>
            <mu-button color="primary" @click="submit">提交</mu-button>
            <mu-button @click="clear">重置</mu-button>
          </mu-form-item>
        </mu-form>
      </mu-paper>
    </mu-container>
  </div>
</template>

<script>
import LoginHeader from "@/components/LoginHeader.vue";
export default {
  name: "Login",
  components: {
    LoginHeader,
  },
  data() {
    return {
      usernameRules: [
        { validate: (val) => !!val, message: "必须填写用户名" },
        { validate: (val) => val.length >= 3 && val.length <= 10, message: "用户名3-10位" },
      ],
      passwordRules: [
        { validate: (val) => !!val, message: "必须填写密码" },
        {
          validate: (val) => val.length >= 3 && val.length <= 10,
          message: "密码3-10位",
        },
      ],
      argeeRules: [{ validate: (val) => !!val, message: "必须同意用户协议" }],
      validateForm: {
        username: "",
        password: "",
        isAgree: true,
      },
    };
  },
  methods: {
    submit() {
      this.$refs.form.validate().then((result) => {
        console.log("form valid: ", result);
        this.$router.push("/Home")
      });
    },
    clear() {
      this.$refs.form.clear();
      this.validateForm = {
        username: "",
        password: "",
        isAgree: false,
      };
    },
  },
};
</script>
<style >
.mpaper {
  background-color: #f5f5f5;
  margin-top: 90px;
  padding: 0 15px;
}
.loginbtn {
  margin-top: 20px;
}
</style>
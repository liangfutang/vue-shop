<template>
    <div>
        <div class="loginOutButton">
            <el-button type="info" @click="loginOut">登出</el-button>
        </div>
    </div>
</template>

<script>
export default {
  methods: {
    loginOut () {
      // 清空token
      window.sessionStorage.removeItem('token')
      // 强制跳转到登录页面
      this.$router.push('/login')
    }
  }
}
</script>

<style lang="less" scoped>
.loginOutButton {
    float: right;
    margin-top:10px;
}
</style>

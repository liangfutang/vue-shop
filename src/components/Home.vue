<template>
    <el-container class="home-container">
      <el-header>
        <div class="loginOutButton">
          <el-button type="info" @click="loginOut">登出</el-button>
        </div>
      </el-header>
      <el-container>
        <el-aside width="200px">Aside</el-aside>
        <el-main>Main</el-main>
      </el-container>
    </el-container>
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

.home-container {
  height: 100%;
}

.el-header {
  background-color: #8f7dca;
}

.loginOutButton {
    float: right;
    margin-top:10px;
    margin-right:15px;
}

.el-aside {
  background-color: #4f5f5f;
}

.el-main {
  background-color: #EAEDF1;
}
</style>

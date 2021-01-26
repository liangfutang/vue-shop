<template>
    <el-container class="home-container">
      <el-header>
        <div>
          <img src="../assets/home-header.jpg" alt="电商后台系统图标" width="10%"/>
          <span>电商后台管理系统</span>
        </div>
        <el-button type="info" @click="loginOut">登出</el-button>
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
  background-color: #373d41;
  display: flex;
  justify-content: space-between;
  padding-left: 0;
  align-items: center;
  color: #fff;
  font-size: 20px;
  > div {
    display: flex;
    align-items: center;
    span {
      margin-left: 15px;
    }
  }
}

.el-aside {
  background-color: #333744;
}

.el-main {
  background-color: #EAEDF1;
}
</style>

<template>
  <div class="login_containter">
    <div class="login_box">
        <!-- 头像区 -->
        <div class="avatar_box">
          <img src="../assets/logo.png" alt="登录表格上面的图标">
        </div>
        <!-- 登录表单区 -->
        <el-form label-width="0px" class="login_form">
          <!-- 用户名 -->
          <el-form-item>
            <el-input prefix-icon="iconfont icon-zhanghao"></el-input>
          </el-form-item>
          <!-- 密码 -->
          <el-form-item>
            <el-input prefix-icon="iconfont icon-mima"></el-input>
          </el-form-item>
          <!-- 登录重置按钮 -->
          <el-form-item class="btns">
            <el-button type="primary">登录</el-button>
            <el-button type="primary">重置</el-button>
          </el-form-item>
        </el-form>
    </div>
  </div>
</template>

<script>
export default { }
</script>

<style lang="less" scoped>
.login_containter{
    background-color: #2b4b6b;
    height: 100%;
}

.login_box{
    width: 450px;
    height: 300px;
    left: 50%;
    top: 50%;
    background-color: #fff;
    border-radius: 12px;
    position: absolute;
    transform: translate(-50%, -50%);
}

.avatar_box{
  width: 130px;
  height: 130px;
  left: 50%;
  border: 1px solid #eee;
  padding: 10px;
  border-radius: 50%;
  box-shadow: 0 0 10px #ddd;
  position: absolute;
  transform: translate(-50%, -50%);
  background-color: #fff;
  img {
    width: 100%;
    height: 100%;
    border-radius: 50%;
    background-color: #eee;
  }
}

.login_form {
  position: absolute;
  bottom: 0;
  width: 100%;
  padding: 0 10%;
  box-sizing: border-box;
}

.btns {
  display: flex;
  justify-content: flex-end;
}
</style>

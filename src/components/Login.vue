<template>
  <div class="login_containter">
    <div class="login_box">
        登录盒子
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
</style>

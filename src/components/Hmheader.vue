<template>
<div class="Hmheader">
    <div class="back">
        <span class="iconfont iconjiantou2"></span>
    </div>
<div class="title"><slot></slot></div>
<div class="extra"></div>
</div>
</template>

<script>
export default {
  back() {
    // this.$router.push()
    // this.$router.back()回退
    // this.$router.forward()
    // this.$router.go(1)前进 正数表示前进
    this.$router.go(-1)
  }
}
</script>

<style lang="less">
.Hmheader{
height:50px;
border-bottom: 1px solid #ccc;
display:flex;
text-align:center;
line-height:50px;
.back,
.extra {
    width:50px
}
.iconfont {
    font-size:16px
}
.title {
    flex:1;
    font-size:18px;
    font-weight:700;
}
}
</style>

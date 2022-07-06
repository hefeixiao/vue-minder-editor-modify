<template lang="html">
  <div class="foot">
    <el-button class="foot-button" id="save-minder" type="primary" @click="saveMinder"> 保存
      <i class="el-icon-upload2 el-icon-right"></i>
    </el-button>
  </div>
</template>
<script>
export default {
  name: 'foot',
  methods: {
    saveMinder: function () {
      this.$emit('saveMinder')
    }
  }
}
</script>

<style scoped>
.foot {
  position: absolute;
  left: 10px;
  height: 35px;
  padding: 5px 0;
  color: #fff;
  border-radius: 4px;
  z-index: 10;
  transition: transform 0.7s 0.1s ease;

  display: flex;
  align-items: center;
  margin: 0;
}
 .foot-button {
   width: 100%;
   float: right;
   height: 30px;
   color: #6495ed;
   background: #fff;
   border-color: #6495ed;
 }

/*按钮悬浮*/
.foot-button:hover {
  background: #e1f3d8 !important;
  color: #6495ed !important;
  font-weight: normal;
  border-color: #01a8f9 !important;
}
/*按钮点击*/
.foot-button:focus {
  background: #6495ed !important;
  color: ghostwhite !important;
  font-weight: normal;
  border-color: #01a8f9 !important;
}
</style>

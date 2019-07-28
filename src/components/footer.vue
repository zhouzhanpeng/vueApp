<template>
    <mt-tabbar v-model="selected">
  <mt-tab-item id="主页">
    <img slot="icon" src="../assets/主页.svg">
    主页
  </mt-tab-item>
  <mt-tab-item id="视频">
    <img slot="icon" src="../assets/视频.svg">
    视频
  </mt-tab-item>
  <mt-tab-item id="我的">
    <img slot="icon" src="../assets/用户.svg">
    我的
  </mt-tab-item>
</mt-tabbar>
</template>
<script>
export default {
    data(){
        return{
        selected:'主页'
            
        }
    }
}
</script>

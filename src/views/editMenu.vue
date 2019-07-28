<template>
 <div>
     <van-icon name="close" />
    <div class="pindao">
    <label class="">我的频道</label>
    <span class="">{{msg}}</span>   
    <span >
        <van-button type="danger" size="mini" round="true" v-show="isedit" @click="edit">编辑</van-button>
        <van-button type="danger" size="mini" round="true"  v-show="!isedit"  @click="editclose">完成</van-button>
    </span>
    </div> 
    <div class="focusChanel" >
     <div class="chanel" v-for="index in focusChanel" :key="index">
      <div class="chanelName">{{index}}</div>
      <div class="chanelclose"><van-icon name="close" /></div>
     </div>


    </div> 
 </div>


</template>
<script>
export default {
    
    data(){
        return{
         msg:'点击进入频道',
         buttonmsg:'编辑',
         isedit:true,
         focusChanel:['关注','推荐','娱乐','生活','影视','情感','视频','中超','国际','杭州','体育','财经','搞笑','经济']
        }
    },
    methods:{
       edit(){
           this.isedit=false
           this.msg='拖拽可以排序'
       },
       editclose(){
           this.isedit=true;
           this.msg='点击进入频道'
       }

    }
    
}
</script>
<style lang="scss" scoped>
@import  '@/assets/scss/editmenu.scss';
</style>

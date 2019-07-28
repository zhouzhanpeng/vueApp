<template>
  <div class="home">
   <search></search>
 

  </div>
</template>

<script>
// @ is an alias to /src
 import headers from '@/components/header.vue'
 import search from '@/components/search.vue'

export default {
  name: 'home',
  components:{
headers,search
  },
  data(){
    return{
      
    }
  },
  methods:{
    gg(){
      alert(3444)
    }
  }

}
</script>

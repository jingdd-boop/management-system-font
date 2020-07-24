<template>
 <div>
   swiper
 </div>
</template>

<script>
import {fetchList} from '@/api/swiper'
export default {
  created(){
    this.getList()
  },
  methods: {
    getList(){
      fetchList().then((res) =>{
        console.log(res)
      })
    }
    
  }
}
</script>

<style>

</style>
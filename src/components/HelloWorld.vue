<template>
  <div class="hello">
    <!-- {{money}} -->
    <!-- <Son1 :money="money"></Son1> -->
    <!-- //子组件通信父组件$emit使用 -->
    父组件：{{money}}
    <Son1 :money="money" @input="change"></Son1>
  </div>
</template>

<script>
import Son1 from '@/components/Son1'
export default {
           methods: {
             change(data){
               this.money=data
             }
           },
           components:{
            Son1
        },
         data(){
          return {money:100}
        },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>

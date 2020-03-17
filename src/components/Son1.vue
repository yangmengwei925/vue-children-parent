<!-- z子组件 -->
<template>
    <div>
        子组件1:{{money}}
        <button @click="$emit('input',200)">修改父组件的值</button><Son1></Son1>
    </div>
</template>

<script>
export default {
  props:{
      value:{
          type:Number,
          default:1
      }
    },
    //如果是数组
    // props:{
    //   value:{
    //     type:Array,
    //     default:()=>[]
    //   }
    // },
  // data () {
  //   return {

  //   };
    
  // },
}

</script>
<style  scoped>

</style>
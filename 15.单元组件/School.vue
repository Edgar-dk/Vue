<template>
<!--1.组件的结构  -->
   <div class="demo">
     <h2>学校名称:{{schoolName}}</h2>
     <h2>学校地址:{{address}}</h2>
     <button @click="showName">点击我提示校名称</button>
   </div>
</template>

<script>
/* 2.组件交互相关的代码（数据，方法等）

     写好这个之后，就可以把这个内容暴露在外面，使用的时候，直接
     import导入就可以了，组件里面的name是暴露在外面，根据这个名字去使用
     
     可以使用简写的方式去定义一个组件*/
export default{
   name:'School',
   data() {
      return {
         schoolName:'Sias',
         address:'郑州'
      }
   },
   methods: {
      showName(){
         alert(this.schoolName)
      }
   },
}
</script>


<style >
/* 3.组件的样式 */
.demo{
   background-color: blue;
}
</style>
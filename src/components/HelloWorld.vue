<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script lang="ts">
/**
  使用vue-class-component后，初始数据可以直接声明为实例的属性，
  而不需放入data() {return{}}中，组件方法也可以直接声明为实例的方法
 */
  import Vue from "vue"
  import Component from 'vue-class-component'
  @Component
  export default class HelloWorld extends Vue{
    msg: string =  'this is a typeScript project now'
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

<template>
  <div>
    <header-component title="리스트페이지"></header-component>
    <div>
      리스트 콘텐츠
      <ul>
        <li v-for="(memo, index) in list" :key="index">{{index}}. {{memo}}</li>
      </ul>
    </div>
    <footer-component></footer-component>
  </div>
</template>

<script>
  export default {
    props:{
      list:{
        type:Array,
        default:[]
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>
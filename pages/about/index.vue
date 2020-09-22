<template>
  <div class="container">
      <h1>about 页面</h1>
      <nuxt-link :to="{name:'index',params:{
        xxid:'9527'
      }}">回首页</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>

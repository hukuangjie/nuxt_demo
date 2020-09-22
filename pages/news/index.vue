<template>
  <div>
    <h1>news 页面</h1>
    <p>newsID：{{$route.params.newsID}}</p>
    <br />
    <ul>
      <li>
        <nuxt-link :to="{name:'index'}">home</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{path:'/news/123'}">news1</nuxt-link>
        <nuxt-link :to="{name:'news-id',params:{
          id:123,title:'i am news'
        }}">news1</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{path:'/news/aaa'}">news2</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  transition:'test'
};
</script>

<style>
</style>

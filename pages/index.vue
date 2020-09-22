<template>
  <div class="container">
    <div>
      <div class="diss">
        <!-- <img src="~static/icon.png" alt /> -->
      </div>
      <h1 class="title">nuxt.js 也就那么回事 {{ $route.params.xxid }}</h1>
      <div class="links">
        <li>
          <nuxt-link :to="{name:'about'}">about</nuxt-link>
        </li>
        <li>
          <nuxt-link :to="{name:'news',params:{
          newsID:10080
        }}">news</nuxt-link>
        </li>
        <li>
          <nuxt-link :to="{name:'asyncData'}">asyncData</nuxt-link>
        </li>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
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
.diss {
  width: 300px;
  height: auto;
  background-image: url('~static/icon.png');
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.links {
  padding-top: 15px;
}
</style>

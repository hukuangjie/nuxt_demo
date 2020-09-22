<template>
  <div>
    <h2>news-content</h2>
    <p>newsID:{{$route.params.id}}</p>
    <ul>
      <li>
        <nuxt-link :to="{name:'index'}">home</nuxt-link>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  validate({ params }) {
    return /^\d+$/.test(params.id);
  },
  data() {
    return {
      title: this.$route.params.title,
    };
  },
  head() {
    return {
      title: this.title,
      meta: [{ hid: "descrition", name: "news1", content: "this is news page" }],
    };
  },
};
</script>
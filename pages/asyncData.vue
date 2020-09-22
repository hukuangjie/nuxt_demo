<template>
  <div>
    <div>姓名:{{info.name}}</div>
    <div>年龄:{{info.age}}</div>
    <div>兴趣:{{info.interest}}</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "hello world",
    };
  },
  async asyncData() {
    let data = await {
      name: "hkj",
      age: 19,
      interest: "学习",
    };
    // return axios.get('./myjson.json').then((res) => {
    return { info: data };
    // });
  },
};
</script>
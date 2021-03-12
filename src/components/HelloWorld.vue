<template>
  <div>
    <h1>当前数字是 {{ msg }}</h1>
    <button @click="zeng">+</button>
    <button @click="jian">-</button>
    <img :src="imageurl" alt="">
    <a :href="jumpurl">百度一下2</a>
  </div>
</template>

<script>
export default({
  data () {
    return {
      msg: 1,
      jumpurl: 'www.baidu.com',
      imageurl: 'https://www.baidu.com/img/PCpad_012830ebaa7e4379ce9a9ed1b71f7507.png'
    }
  },
  methods: {
    zeng () {
      this.msg++
    },
    jian () {
      this.msg--
    }
  }
})
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
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

<!--
 * @Author: @Edwin
 * @Date: 2021-09-23 01:23:10
 * @LastEditors: @Edwin
 * @LastEditTime: 2021-09-23 02:04:36
 * @Description: &1
 * @FilePath: \vue3-independent-develop\vue-demo\src\components\HelloWorld.vue
-->
<template>
  <div>Hello</div>
  <div>World</div>
</template>

<script>
import { onMounted } from 'vue'

function test() {
  onMounted(() => {
    console.log('mounted')
  })
}

export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
  setup() {
    test()
  },
  data() {},
  methods: {},
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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

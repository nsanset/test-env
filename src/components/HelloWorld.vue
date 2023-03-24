<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>{{ testEnv }}</h2>
    <h2>{{ testEnv2 }}</h2>
    <h2>{{ testEnv3 }}</h2>
    <h2>{{ testEnv4 }}</h2>
  </div>
</template>

<script>
const test = process.env.ROOT_API
const test2 = process.env.R_APPS
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      testEnv: process.env.ROOT_API,
      testEnv2: test,
      testEnv3: process.env.R_APP,
      testEnv4: test2
    }
  }
  // mounted() {
  //   console.log(process.env.ROOT_API)
  // }
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

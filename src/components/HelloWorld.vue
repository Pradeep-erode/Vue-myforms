<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <label for="">Type here and enter and see console: (keyup - enter modifiers  used here )</label>
    <input v-model="myval" @keyup.enter="subtract()"/>
  </div>
</template>

<script>
// const privateEnvVar = import.meta.env.VITE_MY_ENV_VARIABLE;
const ask = '';
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
    return{
      myval:''
    }
  },
  methods:{
  subtract(){
    console.log(this.myval),
    this.myval=ask
  }
}
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

<template>
<h1>{{msg}}</h1>
<button @click="genRanNum()">Generate random Numbers</button>
<h2>{{random_number}}</h2>
</template>

<script>
export default {
  name: 'RandomNumber',

  data(){
    return{
    random_number:0
    }
  },

  props: {
    msg: String,
    min:{type: Number, default: 1},
    max:{type: Number, default: 10}
  },

  methods:{
    genRanNum(){
      this.random_number = Math.floor(Math.random() * (this.max - this.min + 1) + this.min) // generate random number from 1 to 100
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

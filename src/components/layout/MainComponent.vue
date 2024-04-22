<template>
  <div>
    <p>Count: {{ count }}</p>
    <p>Message: {{ message }}</p>
    <button @click="incr">Increment Count</button>
  </div>
</template>

<script>
import { watch } from 'vue';

export default {
  data() {
    return {
      count: 0,
    };
  },
  props: {
    message: String,
  },
  watch: {
    count(newVal, oldVal) {
      console.log(newVal, oldVal);
    }
  },
  
  methods: {
    incr() {
      this.count++;
    }
  }
}
</script>



<style scoped>
.hello{
    display: flex;
    justify-content: center;  
    font-size: 10px;
    background-color: white ;
    
}
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

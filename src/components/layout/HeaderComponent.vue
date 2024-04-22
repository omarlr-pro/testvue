<template>
  <div class="hello">
    <h1>{{ compteur }}</h1>
    <button @click="incr">Increment</button>
    <button @click="decrement">Decrement</button>
  </div>
</template>
>

<script>
export default {
  data() {
    return {
      compteur: 0 
    };
  },
  methods: {
    incr() {
      this.compteur++;
    },
    decrement() {
      this.compteur--;
    }
  }
};
</script>

<style scoped>
.hello {
  color: black;
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

<template>
  <div class="hello">
    <h1>{{message}}</h1>
   <h2>hihi</h2>
   <h3>{{fullName}}</h3>
  </div>
</template>

<script>
export default {
  data() {
    return {
      firstName: 'Omar',
      lastName: 'Lar',
    };
  },
  computed: {
    fullName() {
      return this.firstName + ' ' + this.lastName;
    },
  },
  props: {
    message: String,
  },
};

</script>

<style scoped>
.hello {
  color: red;
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

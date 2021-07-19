<template>
  <div class="hello">
    <h1 v-on:click="show">TODOs</h1>
    <ol>
      <li v-for="item in items" :key="item.id">
        {{ item.name }}
      </li>
    </ol>
  </div>
</template>

<script>
export default {
  name: "Todos",
  props: {
    items: Array,
  },
  data() {
      return {
          msg: "Here"
      }
  },
  methods:{
      show:function() {
          alert("Total todos: " + this.items.length);
      }
  },
  
};
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

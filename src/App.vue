<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <Todos :items="items" />
</template>

<script>
import Todos from "./components/todos.vue";

export default {
  name: "App",
  data() {
    return {
      items: [
        {
          name: "item - 1",
          finished: false,
        },
      ],
    };
  },
  components: {
    Todos,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

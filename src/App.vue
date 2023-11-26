<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Welcome to Your Vue.js App" /> -->
  <div id="header">
    Todo-Board
  </div>
  <div id="todos">
    <base-todo-card title="Test Todo">
    </base-todo-card>
    <daily-view>
    </daily-view>
  </div>
</template>

<script>
import BaseTodoCard from "./components/base-components/BaseTodoCard.vue"
import DailyView from './components/DailyView.vue';

export default {
  name: "App",
  components: {
    BaseTodoCard,
    DailyView
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
}

#header {
  height: 100px;
  width: 100%;
  font-size: 25pt;
  display: flex;
  align-items: center;
  justify-content: center;
  color: lightsalmon;
  background-color: #2c3e50;
}
</style>

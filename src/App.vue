<template>
  <div>
    <h1>Як передати із одного компонента в другий не використовуючи props</h1>
    <app-head></app-head>
  </div>
</template>

<script>
import appHead from "./components/header";
export default {
  name: "App",
  provide: {
    title: "Ось так привіт Світ: I`m Yevhenii",
  },
  components: {
    appHead,
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

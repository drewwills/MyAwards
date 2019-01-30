<template>
  <div id="app">
    <i class="material-icons md-48"> assignment </i> <MyAwards />
  </div>
</template>

<script>
import MyAwards from './components/MyAwards';

export default {
  name: 'App',
  components: {
    MyAwards,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.material-icons.md-48 {
  font-size: 48px;
}
.material-icons.md-64 {
  font-size: 64px;
}
</style>

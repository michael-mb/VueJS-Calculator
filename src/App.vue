<template>
  <h3 class="big-title">Vue JS Calculator</h3>
  <calculator></calculator>
</template>

<script>
import Calculator from "@/components/Calculator";
export default {
  name: 'App',
  components: {
    Calculator

  }
}
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

body {
  max-width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: sans-serif;
  background-image: linear-gradient(to top, #a18cd1 0%, #fbc2eb 100%);
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.big-title{
  font-size: 25px;
  margin: 15px;
  color: crimson;
}
</style>

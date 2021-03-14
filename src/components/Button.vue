<template>
  <button @click="$emit('clicked' , text)" class="button">{{text}}</button>
</template>

<script>
export default {
  name: "Button",
  props:{
    text: String,
  }

}
</script>

<style scoped>
button {
  border: none;
  outline: none;
  border-radius: 5px;
  background-color: #f7f7f7;
  box-shadow: 0 3px #a8a8a8;
  font-size: 18px;
}

button:active {
  box-shadow: 0 1px #a8a8a8;
  transform: translateY(2px);
}
</style>
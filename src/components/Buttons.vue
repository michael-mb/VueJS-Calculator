<template>
  <div class="buttons">
    <Button @clicked="$emit('btnClicked', 'C')" style="  background-color: #ff9900;font-weight: bold;color: white;" text="C"></Button>
    <Button @clicked="$emit('btnClicked', '(')" text="("></Button>
    <Button @clicked="$emit('btnClicked', ')')" text=")"></Button>
    <Button @clicked="$emit('btnClicked', '/')" text="/"></Button>
    <Button @clicked="$emit('btnClicked', '7')" text="7"></Button>
    <Button @clicked="$emit('btnClicked', '8')" text="8"></Button>
    <Button @clicked="$emit('btnClicked', '9')" text="9"></Button>
    <Button @clicked="$emit('btnClicked', '*')" text="*"></Button>
    <Button @clicked="$emit('btnClicked', '4')" text="4"></Button>
    <Button @clicked="$emit('btnClicked', '5')" text="5"></Button>
    <Button @clicked="$emit('btnClicked', '6')" text="6"></Button>
    <Button @clicked="$emit('btnClicked', '-')" text="-"></Button>
    <Button @clicked="$emit('btnClicked', '1')" text="1"></Button>
    <Button @clicked="$emit('btnClicked', '2')" text="2"></Button>
    <Button @clicked="$emit('btnClicked', '3')" text="3"></Button>
    <Button @clicked="$emit('btnClicked', '+')" text="+"></Button>
    <Button @clicked="$emit('btnClicked', '0')" text="0"></Button>
    <Button @clicked="$emit('btnClicked', '.')" text="."></Button>
    <Button @clicked="$emit('btnClicked', '=')" style="  grid-column: span 2;  background-color: #36e700;font-weight: bold;color: white;" text="="></Button>




  </div>

</template>

<script>
import Button from "@/components/Button";
export default {
name: "Buttons",
  components: {Button}
}
</script>

<style scoped>
.buttons {
  display: grid;
  grid-template-columns: repeat(4, 50px);
  grid-template-rows: repeat(5, 50px);
  grid-gap: 7px;
}
</style>
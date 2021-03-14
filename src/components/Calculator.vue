<template>
  <div class="calculator">
    <div class="screen">{{screenText}}</div>
    <Buttons @btnClicked="btnClicked"></Buttons>
  </div>
</template>

<script>
import Buttons from "@/components/Buttons";
export default {
name: "Calculator",
  components: {Buttons},
  data() {
    return {
      screenText : '',
    }
  },
  methods:{
    btnClicked(text){
      if(text === 'C')
        this.screenText = ''
      else if(text === '=')
        this.screenText = eval(this.screenText)
      else
        this.screenText += text
    },
  }
}

window.addEventListener('error', (e) => {
  alert('Error : ' + e.message)
})
</script>

<style scoped>
.calculator{
  background-color: #222222;
  display: flex;
  flex-direction: column;
  padding: 15px;
  border-radius: 5px;
  box-shadow: 0 5px black;
}
.screen{
  width: 100%;
  height: 100px;
  background-color: rgb(198, 237, 255);
  margin-bottom: 10px;
  border-radius: 5px;
  display: flex;
  justify-content: flex-end;
  align-items: flex-end;
  padding: 5px;
  font-size: 25px;
}
</style>
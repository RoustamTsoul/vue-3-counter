<template>
 <div id="app">
    <div class="conteiner">
      <Counter/>
    </div>
 </div>
</template>

<script>
import Counter from './components/Counter.vue'

export default {
  name: 'App',
  components: {
    Counter
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Rubik+Gemstones&display=swap');

body{
  font-family: 'Rubik Gemstones', cursive;
  color: goldenrod;
  background:linear-gradient(90deg, rgba(255, 255, 0, 1) 6%, rgba(255, 235, 59, 1) 30%, rgba(233, 30, 99, 1) 53%, rgba(238, 130, 238, 1) 100%);
}
#app{
  margin-top:150px;
}
.container{
    width: 95%;
    height: 100vh;
    margin: auto;
    display: flex;
    justify-content: center;
    align-items: center;
}


</style>

<template>
<div class="home">
  <img alt="Vue logo" src="./assets/logo.png">
  <div class="counter">
    {{  counter }}
  </div>
  <div class="buttons">
    <button @click="decreaseCounter">-</button>
    <button @click="increaseCounter">+</button>
  </div>
</div>

</template>

<script>

export default {
  name: 'App',
  components: {
  
  },
  data(){
    return {
      counter: 0
    }
  }, 
  methods: {
    increaseCounter() {
      this.counter++
    },
    decreaseCounter() {
      this.counter--
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.home {
  margin-bottom: 10px;
}
.counter {
font-size: 80px;
}

.buttons button {
  font-size: 40px;
  width: 100px;
  margin: 0 10px;
}
</style>

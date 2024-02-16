<template>
  <div class="home">
    <img alt="Vue logo" src="./assets/logo.png">
    <div class="counter">
      {{  $store.state.counter }}
    </div>
    <div class="buttons">
      <button @click="decreaseCounter">-</button>
      <button @click="increaseCounter">+</button>
    </div>
  </div>
  
  </template>
  
  <script>

import store from './store'; 
  
  export default {
    name: 'App',
    methods: {
      decreaseCounter() {
        this.counter--
      },
      increaseCounter() {
        this.counter++
      }
    },
    store
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
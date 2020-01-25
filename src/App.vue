<template>
  <div id="app">
<!--    <img alt="Vue logo" src="./assets/logo.png">-->
    <choice-field>  </choice-field>
    <color-field/>
  </div>
</template>

<script>

import ChoiceField from "@/components/choiceField";
import ColorField from "@/components/HelloWorld";

export default {
  name: 'app',
  components: {
      ChoiceField,
      ColorField
  }
}
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    padding-top: 60px;
    height: 100%;
  }

  .colorField {
    height: 80%;
    width: 100%;
  }

  html  {
    height: 100%;
  }

  body  {
    height: 100%;
  }
</style>

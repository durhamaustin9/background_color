<template>
    <div class="choice" id="box">
      <i class="fas fa-sliders-h" id="settings">  </i>

        <h1>Choose a Color</h1>

        <button class="btn btn-success" id="gButton" v-on:click="gButton">Green</button>

        <button class="btn btn-danger" id="rButton" v-on:click="rButton">Red</button>
    </div>
</template>

<script>
    export default {
        name: "choiceField",
        methods: {
            gButton: function () {
              let select = document.getElementById('colorBox');

              select.style.backgroundColor = 'green';
            },

            rButton: function () {
              let select = document.getElementById('colorBox');

              select.style.backgroundColor = 'red';
            }
        }
    }
</script>

<style scoped>
    #gButton  {
      color: whitesmoke;
      font-size: 2em;
      background-color: green;
      margin-right: 10px;
    }

  #rButton  {
    color: whitesmoke;
    font-size: 2em;
    background-color: red;
    margin-right: 10px;
  }

  .choice {
    min-width: 360px;
    height: 20%;
  }

  #settings {
    font-size: 2rem;
    position: absolute;
    right: 5%;
  }
</style>
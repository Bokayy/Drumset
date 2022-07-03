<template>
  <div id="app">
    <div id="drumkit">
      <img alt="Drums" src="./assets/Garageband.jpg">
      <button id="drumkit__instrument" class="crash">R</button>
      <button id="drumkit__instrument" class="tomtom1">T</button>
      <button id="drumkit__instrument" class="tomtom2">U</button>
      <button id="drumkit__instrument" class="ride">I</button>
      <button id="drumkit__instrument" class="hihat">F</button>
      <button id="drumkit__instrument" class="snare">V</button>
      <button id="drumkit__instrument" class="kick">B</button>
      <button id="drumkit__instrument" class="floortom">N</button>
    </div>
  </div>
</template>

<script>

export default {
  name: 'App',

  data() {
  },
}
</script>

<style scoped lang="scss">
body {
  margin: 0;
  padding: 0;
  height: 100%;
  width: 100%;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

  #drumkit{
    position: relative;
    max-height: 95vh;

    img{
      object-fit: cover;
      height: 99.5vh;
    }

    &__instrument{
      $self: &;
      height: 5rem;
      width: 5rem;
      position: absolute;
      border: 3px solid white;
      border-radius: 5px;
      font-size: 1.5rem;
      background-color: rgb(75, 75, 75);
    }

    &--active{
      border: yellow 5px solid;
      text-shadow: 0px 0px 35px yellow;
    }

    .crash{
      top: 12rem;
      left: 13rem;
    }

    .tomtom1{
      top:20rem;
      left:38rem;
    }
    .tomtom2{
      top:20rem;
      left:64rem;
    }
    .ride{
      top: 13rem;
      left: 90rem;
    }

    .hihat{
      top: 30rem;
      left:13rem;
    }

    .snare{
      top:50rem;
      left: 20rem;
    }
    .kick{
      top:50rem;
      left: 51rem;
    }
    .floortom{
      top:50rem;
      left: 85rem;
    }
  }
}
</style>

<template>
  <div id="app">
    <img alt="Drums" src="./assets/Garageband.jpg">
  </div>
</template>

<script>

class DrumKey {
//properties
template = `
   <button class = ${this.instrument}>

   </button>
`;
//properties


//methods

//methods

}


export default {
  name: 'App',
  data() {
    // eslint-disable-next-line no-unused-labels
    Snare: new DrumKey();
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

  img{
    object-fit: cover;
    height: 100vh;
  }

}
</style>

<template>
  <div id="app">
  <img src="src/assets/logo.png">
    <ul v-for="person in persona">
      <li>Nombre de persona: {{ person.name }}</li>
      <li>Apellido de persona: {{ person.lastName }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      persona: [
        { 
          name: 'Wander', 
          lastName: 'Lindao' 
        },
        { 
          name: 'Jorge', 
          lastName: 'Diaz' 
        },
        { 
          name: 'Juan', 
          lastName: 'Caicedo' 
        }
      ] 
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>

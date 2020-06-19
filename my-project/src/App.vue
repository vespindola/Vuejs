<template>
  <div id="app" class="comp">
    <h2>{{title}}</h2>
  <h1> {{ msg }} </h1>
  <br>
  <teste-components></teste-components>
  <br>
  <form-components></form-components>
  <br>
  <tasks-components></tasks-components>
  </div>
</template>

<script>
import TesteComponents from './Components/TesteComponents'
import FormComponents from './Components/FormComponents'
import TasksComponents from './Components/TasksComponents'
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App by Integrado',
      title: 'AppComponent'
    }
  },
  components: {
    TesteComponents,
    FormComponents,
    TasksComponents

  }
}
</script>

<style>
.comp{border: 1px solid blue; margin: 5px; padding: 5px;}
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

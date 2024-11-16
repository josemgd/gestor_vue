<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Esta pagina web permite gestionar tus tareas, cargando una lista existente, añadiendo nuevas<br>
      tareas a dicha lista, marcando como completa o no<br>
      Para ver mis otros proyectos visita mi github!
      <a href="https://github.com/josemgd" target="_blank" rel="noopener"> AQUI<i class="bi bi-github"></i></a>.
    </p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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

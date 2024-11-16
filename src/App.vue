<template>
  <div id="app">
    <!-- Barra de navegación responsiva -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark custom-navbar">
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- Contenedor de los enlaces de navegación -->
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item">
            <router-link class="navbar-brand" to="/"><i class="bi bi-house-door-fill"></i>Home</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/addtask"><i class="bi bi-plus"></i>Agregar Tarea</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/tasklist"><i class="bi bi-card-checklist"></i>Lista de Tareas</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/combinedview"><i class="bi bi-columns"></i>Vista Combinada</router-link>

          </li>
        </ul>
      </div>
    </nav>

    <!-- El componente cargado de acuerdo a la ruta -->
    <router-view />
  </div>
</template>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

/* Personalización del navbar */
.custom-navbar {
  padding: 10px 20px;
  background-color: #1a2c54; /* Color de fondo */
}

.custom-navbar .navbar-brand {
  color: rgb(238, 238, 238) !important;
  font-weight: bold;
  font-size: 1.5rem;
}

.custom-navbar .navbar-brand:hover {
  color: #4d7b93 !important;
}

.custom-navbar .nav-link {
  color: white !important; /* Color de enlaces */
}

.custom-navbar .nav-link:hover {
  color: #4d7b93 !important; /* Color al pasar el mouse */
}

/* Estilo cuando el enlace está activo */
.custom-navbar .router-link-exact-active {
  color: #4d7b93 !important;
  font-weight: bold;
}
</style>
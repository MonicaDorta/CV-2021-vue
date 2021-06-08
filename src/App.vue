<template>
  <div class="content">
    <Menu/>
    <div class="datos">
      <Datos nombre='Mónica' apellidos='Dorta Escobar'/>
      <Educacion/>
      <Experiencia/>
      <Aptitudes/>
      <Proyectos/>
    </div>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Datos from './components/Datos.vue'
import Menu from './components/Menu.vue'
import Educacion from './components/Educacion.vue'
import Experiencia from './components/Experiencia.vue'
import Aptitudes from './components/Aptitudes.vue'
import Proyectos from './components/Proyectos.vue'

export default {
  name: 'App',
  components: {
    Datos,
    Menu,
    Educacion,
    Experiencia,
    Aptitudes,
    Proyectos
  }
}
</script>

<style lang="scss" scope>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.content{
  display: flex;
}

.datos{
  height: 100vh;
}

</style>

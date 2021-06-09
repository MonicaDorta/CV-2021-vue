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
import Datos from './views/Datos.vue'
import Menu from './views/Menu.vue'
import Educacion from './views/Educacion.vue'
import Experiencia from './views/Experiencia.vue'
import Aptitudes from './views/Aptitudes.vue'
import Proyectos from './views/Proyectos.vue'

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

.container{
    margin-left: 20rem;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    min-height: 100vh; 

    h1 {
        text-transform: uppercase;
        font-weight: 650;
        font-size: 4rem;
        color:#343a40;
        margin-bottom: 4rem;
        padding-top:8rem;
    }  
  }

</style>

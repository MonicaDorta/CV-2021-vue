<template>
  <div class="container" id="experiencia">
      <h1>Experiencia Laboral</h1>
      <div v-for="item in items" :key="item">
        <Listado :cat="categoria" :titulo="item.empresa" :subtitulo="item.fecha" :contenido="item.tareas"/>
        <hr>
      </div>
  </div>
</template>

<script>
import Listado from '../components/Listado.vue'

export default {
    name: 'Experiencia',
    components: {
      Listado
    },
    data(){
      return{
        categoria:'experiencia',
        items: [
          {
            empresa: 'CARTELING.COM – Diseñadora gráfica', 
            fecha: 'Junio 2018 – Febrero 2020', 
            tareas:[
              'Desarrollo de cartelería en cada una de sus fases, desde el diseño hasta su producción.', 
              'Labores administrativas y atención al cliente.',
              'Desempeño en la página web para la introducción de productos.'] 
          },
          {
            empresa: 'STV CANARIAS – Desarrolladora Web', 
            fecha: 'Septiempre 2020 – Noviembre 2020', 
            tareas:[
              'Becaria en el departamento de coordinación.',
              'Coordinación de equipo y call center.',
              'Desarrollo de herramientas que facilitan el trabajo del departamento en PHP.'
            ]
          },
          {
            empresa: 'AONIA SOFTWARE S.L – Técnica informática', 
            fecha: 'Noviembre 2020 – Febrero 2021', 
            tareas:[
              'Desarrollo de herramientas educativas (SCORM).',
              'Creación de minijuegos infantiles en JavaScript.'
            ] 
          },
          {
            empresa: 'ADVENTUREES ALLIANCE S.L – Técnica informática', 
            fecha: 'Febrero 2020 – Marzo 2021', 
            tareas:[
              'Maquetación de páginas web en Adobe XD.',
              'Desarrollo Front-end con Vue.js.'
            ] 
          }
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
  
</style>  

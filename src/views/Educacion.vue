<template>
  <div class="container" id="educacion">
      <h1>Educación</h1>
      <div v-for="item in items" :key="item">
        <Listado :cat="categoria" :titulo="item.centro" :subtitulo="item.fecha" :contenido="item.estudio"/>
        <hr>
      </div>
  </div>
</template>

<script>
import Listado from '../components/Listado.vue'

export default {
    name: 'Educacion',
    components: {
      Listado
    },
    data(){
      return{
        items: [
          {centro: 'IES La Laboral de La Laguna', fecha: 'Finalizado en 2011', estudio: ['Bachillerato científico-tecnológico.']},
          {centro: 'CIFP César Manrique', fecha: 'Finalizado en 2019', estudio: ['Ciclo Superior en Desarrollo de aplicaciones Web de manera presencial.']},
          {centro: 'CIP La Laguna', fecha: 'Finalizado en 2020', estudio: ['Finalización del Ciclo Superior en Desarrollo de aplicaciones Web a distancia.']}
        ],
        categoria: 'estudio'
      }
    }
}
</script>

<style lang="scss" scoped>
  
</style>  
<template>
  <div class="container" id="experiencia">
    <h1>Experiencia laboral</h1>
    <div v-for="item in items" :key="item">
      <div class="experiencia">
        <h2>{{item.empresa}}</h2>
        <h3>{{item.fecha}}</h3>  
        <ul v-for="tarea in item.tareas" :key="tarea">
            <li>{{tarea}}</li>              
        </ul>  
      </div>
      <hr>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Datos',
    data(){
      return{
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

    .experiencia{
        margin: 3rem;
        h2{
            line-height: 0;
            font-size: 2rem;
            color:#343a40;

            span{
                color: cadetblue;
                font-weight: 600;
                font-size: 1.2rem;
                margin: 0.3rem;
            }
        }

        h3{
            color: cadetblue;
            font-size: 1rem;
        }

        li{
            color:#7c7e80;
            font-size: 1.5rem;
            width: 70%;
        }
    }
  }
</style>  
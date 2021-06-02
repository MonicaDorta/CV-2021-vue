<template>
  <div class="container" id="experiencia">
      <h1>Experiencia laboral</h1>
      <div class="experiencia">
        <h2>CARTELING.COM – Diseñadora gráfica</h2>
        <h3>Junio 2018 – Febrero 2020</h3>  
        <ul>
            <li>Desarrollo de cartelería en cada una de sus fases, desde el diseño hasta su producción.</li>
            <li>Labores administrativas y atención al cliente.</li>
            <li>Desempeño en la página web para la introducción de productos.</li>
        </ul>  
      </div>
      <hr>
      <div class="experiencia">
        <h2>STV CANARIAS – Desarrolladora Web</h2>
        <h3>Septiempre 2020 – Noviembre 2020</h3>    
        <ul>
            <li>Becaria en el departamento de coordinación.</li>
            <li>Coordinación de equipo y call center.</li>
            <li>Desarrollo de herramientas que facilitan el trabajo del departamento en PHP.</li>
        </ul>
      </div>
      <hr>
      <div class="experiencia">
        <h2>AONIA SOFTWARE S.L – Técnica informática</h2>
        <h3>Noviembre 2020 – Febrero 2021</h3>   
        <ul>
            <li>Desarrollo de herramientas educativas (SCORM).</li>
            <li>Creación de minijuegos infantiles en JavaScript.</li>
        </ul> 
      </div>  
      <hr>
      <div class="experiencia">
        <h2>ADVENTUREES ALLIANCE S.L – Técnica informática</h2>
        <h3>Febrero 2020 – Marzo 2021</h3>    
        <ul>
            <li>Maquetación de páginas web en Adobe XD.</li>
            <li>Desarrollo Front-end con Vue.js.</li>
        </ul>
      </div>   
  </div>
</template>

<script>
export default {
    name: 'Datos',
    props: {
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
<template>
  <div class="container" id="educacion">
      <h1>Educación</h1>
      <div class="estudio">
        <h2>IES La Laboral de La Laguna</h2>
        <h3>Finalizado en 2011</h3>    
        <p>Bachillerato científico-tecnológico.</p>
      </div>
      <hr>
      <div class="estudio">
        <h2>CIFP César Manrique</h2>
        <h3>Finalizado en 2019</h3>    
        <p>Ciclo Superior en Desarrollo de aplicaciones Web de manera presencial.</p>
      </div>
      <hr>
      <div class="estudio">
        <h2>CIP La Laguna</h2>
        <h3>Finalizado en 2020</h3>    
        <p>Finalización del Ciclo Superior en Desarrollo de aplicaciones Web a distancia.</p>
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

    .estudio{
        margin: 3rem;
        h2{
            text-transform: uppercase;
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

        p{
            color:#7c7e80;
            font-size: 1.5rem;
            width: 70%;
        }
    }
  }
</style>  
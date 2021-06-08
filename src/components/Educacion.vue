<template>
  <div class="container" id="educacion">
      <h1>Educación</h1>
      <div v-for="item in items" :key="item">
        <div class="estudio">
          <h2>{{item.centro}}</h2>
          <h3>{{item.fecha}}</h3>    
          <p>{{item.estudio}}</p>
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
          {centro: 'IES La Laboral de La Laguna', fecha: 'Finalizado en 2011', estudio: 'Bachillerato científico-tecnológico.'},
          {centro: 'CIFP César Manrique', fecha: 'Finalizado en 2019', estudio: 'Ciclo Superior en Desarrollo de aplicaciones Web de manera presencial.'},
          {centro: 'CIP La Laguna', fecha: 'Finalizado en 2020', estudio: 'Finalización del Ciclo Superior en Desarrollo de aplicaciones Web a distancia.'}
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
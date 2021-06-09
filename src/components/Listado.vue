<template>
  <div v-bind:class="cat">
    <h2>{{titulo}}</h2>
    <h3>{{subtitulo}}</h3>  
    <ul v-for="cont in contenido" :key="cont">
        <li>{{cont}}</li>              
    </ul>  
  </div>
</template>

<script>
export default {
    name: 'Listado',
    props: {
        titulo: String,
        subtitulo: String,
        contenido: String,
        cat:String
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

    .experiencia, .estudio{
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
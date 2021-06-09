<template>
  <div class="container" id="aptitudes">
      <h1>Aptitudes</h1>
      <div class="aptitud">
          <h2>IDIOMAS</h2>
          <p><img src="../assets/ing.png"> -  Nivel medio</p>
      </div>
      <hr>
      <div class="aptitud">
          <h2>INFORMÁTICA</h2>
          <div class="lenguajes">
              <img v-for="item in array" :key="item" v-bind:src="require('../assets/icons/' + item + '.png')" alt="">
          </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Datos',
    data(){
        return {
            array:["bootstrap", "composer", "css3", "html5", "java", "javascript", "jquery", "laravel", "mysql", "php", "sass"]
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

    .aptitud{
        margin: 3rem;
        img{
            width: 1.5rem;
            margin-right: 10px;
        }
        .lenguajes img{
            width: 2.5rem;
        }
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
            margin: 3rem;
            color:#7c7e80;
            font-size: 1.5rem;
            width: 70%;
            display: flex;
            align-items: center;
        }
    }
  }
</style>  
<template>
  <div class="container" id="perfil">
    <h1>{{nombre}} <span>{{apellidos}}</span></h1>
    <h2>Desarrolladora Web <span> · </span> 662 118 579 <span> · </span> monicadortaescobar@gmail.com</h2>
    <p>Me considero una persona creativa, perfeccionista y curiosa, con ganas de aprender cosas nuevas que me ayuden a desempeñar mi trabajo de la mejor manera posible. Soy una programadora Junior trabajadora, con recursos, sociable y con capacidad para trabajar en equipo.</p>
    <div class="redes">
        <a class="social-icon" href="#"><i class="fab fa-linkedin-in"></i></a>
        <a class="social-icon" href="#"><i class="fab fa-github"></i></a>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Datos',
    props: {
      nombre: String,
      apellidos:String
    }
}
</script>

<style lang="scss" scoped>
  .container{
    margin-left: 20rem;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    min-height: 100vh; 

    .social-icon {
      padding: 0.5rem;
      background-color: #495057;
      color: #fff;
      border-radius: 100%;
      font-size: 1.5rem;
      margin-right: 1.5rem;

      &:hover{
        background-color: cadetblue;
      }
    }

    span{
      color:cadetblue;
    }

    h1 {
      padding-top: 15rem;
      text-transform: uppercase;
      font-weight: 650;
      font-size: 5rem;
      color:#343a40;
      margin-bottom: 0;
    }    

    h2{
      text-transform: uppercase;
      line-height: 0;
      font-size: 1rem;
      margin-bottom: 3rem;
      color:#7c7e80;

      span{
        color: cadetblue;
        font-weight: 600;
        font-size: 1.2rem;
        margin: 0.3rem;
      }
    }

    p{
      font-size: 1.5rem;
      color:#343a40;
      width: 70%;
    }
  }
</style>  
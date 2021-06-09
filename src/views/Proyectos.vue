<template>
  <div class="container" id="proyectos">
      <h1>Proyectos</h1>
      <div class="grid">
        
        </div>
  </div>
</template>

<script>
export default {
    name: 'Proyectos',
    props: {
    }
}
</script>

<style lang="scss" scoped>
  .container{
    margin-left: 20rem;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    min-height: 100vh; 

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
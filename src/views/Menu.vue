<template>
  <div class="menuTab">
    <img alt="Mónica Dorta Escobar" src="../assets/CV.jpg">
    
    <nav class="navbar">
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav">
                <li class="nav-item"><a class="nav-link js-scroll-trigger" href="#perfil">Perfil</a></li>
                <li class="nav-item"><a class="nav-link js-scroll-trigger" href="#educacion">Educación</a></li>
                <li class="nav-item"><a class="nav-link js-scroll-trigger" href="#experiencia">Experiencia laboral</a></li>
                <li class="nav-item"><a class="nav-link js-scroll-trigger" href="#aptitudes">Aptitudes</a></li>
                <li class="nav-item"><a class="nav-link js-scroll-trigger" href="#proyectos">Proyectos</a></li>
            </ul>
        </div>
    </nav>
  </div>
</template>

<script>
export default {
    name: 'Menu',
    props: {

    }
}
</script>

<style lang="scss" scoped>
    .menuTab{
        background-color:cadetblue;
        position: fixed;
        font-weight: 750;
        letter-spacing: 0.05rem;
        text-transform: uppercase;
        height: 100vh;
        text-align: center;
        padding-top: 15rem;
        width: 17rem;
    }
    a{
        text-decoration: none;
        color: whitesmoke;
        opacity: 0.7;
        &:hover{
            opacity: 1;
        }
    }
    li{
        list-style:none;
        margin: 20px;
    }
    .navbar {
        list-style: none; 
        ul{
          padding: 0px;  
        }
    }
    img{
        width: 150px;
        border: 7px solid rgb(125, 192, 194);
        border-radius: 100%;
    }
</style>
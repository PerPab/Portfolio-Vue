<template>
<div class="container-fluid d-flex flex-column align-items-center justify-content-start m-0 p-0 about">
    <h5 class="text-center mt-1">Sobre Mi</h5>
    <img class="img-fluid profile  " src="img/prof-d-b2.png"/>
    <div class="container container-text p-4 animate__animated animate__bounceIn">
        <p class="text-center">Me llamo Pablo, soy estudiante de las carreras de
        Desarrollo de Software en ISTEA y Administración de Empresas en UTN, y durante el año 2022 obtuve el título de Auxiliar en Programación.
            Actualmente me desempeño como Programador Jr. en una empresa de Software.
        Me gusta la música, dibujar, la
        edición de
        imágenes y diseñar logos e interfaces de usuario.
    </p>

    </div>
</div>

</template>

<script setup></script>

<style scoped>
p{
    user-select: none;
}
h5{
    color: #F8F9FA;
    user-select: none;
}
.about{
    width: 100%;
    height: calc(100vh - 86px);
    overflow-y: hidden; 
    overflow-x: hidden; 
    background-color: #28292A;
}

.container-text{
    width: 50%;
    background-color: #F8F9FA;
    font-size: 1.2rem;
    font-weight: 100;
    border-radius: 10px;


}
.profile{
    width: 160px;
    border-radius: 50%;
    background-color: #F8F9FA;
    border-radius: 10px;
    margin: 2%;
}

@media (max-width: 720px){
    .container-text{
    width: 90%;
    font-size: 1.1rem;
    font-weight: 400;

}

.profile{
    width: 120px;
    margin-top: 1rem;
    margin-bottom: 2rem;
    
}



}


</style>

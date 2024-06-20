<template>
    <div class="container-fluid d-flex flex-column align-items-center justify-content-start m-0 p-0 about">
        <h5 class="text-center mt-1">Proyectos</h5>
        <div class="contenedor ">
            <div v-for="item in info" v-bind:key="item.title" class="p-0 m-0 card-container animate__animated animate__bounceIn">
            <ProjectCard :title="item.title" :description="item.description" :link="item.link" />
            </div>

        </div>

        
    </div>
</template>
    
<script setup>
import ProjectCard from './ProjectCard.vue';

let info = [{
    title: "Gestor de inventarios",
    description: "Una aplicación de escritorio que se conecta a una base de datos SQLite y permite realizar operaciones CRUD sobre las tablas. Desarrollada con WPF, C#, y SQLite.",
    link: 'https://github.com/PerPab/GestorInventarioSQL'
},
{
    title: "Generador de gráficos",
    description: "Esta App genera un gráfico de datos previamente ingresados, permite seleccionar tipo de gráfico y descargar una imagen del mismo.",
    link: 'https://perpab.github.io/Generador-Grafico/'
},
{
    title: "To Do list con voz",
    description: "Una App para guardar tareas, almacena las notas en una API y utiliza Speech Synthesis para leerlas, permite configurar idioma y velocidad.",
    link: 'https://perpab.github.io/parcial_2_PWA/'

},
{
    title: "Explorador de Archivos",
    description: "Un explorador de archivos desarrollado en C# y WPF. Permite buscar, abrir, crear y eliminar ficheros.",
    link: 'https://github.com/PerPab/ExploradorArchivos'

},
{
    title: "Creador de personajes",
    description: "Una prueba realizada en Vue para experimentar con la reactividad de los elementos.",
    link: 'https://prueba-reactividad-vue.vercel.app/'

},
{
    title: "Monitor de Hardware",
    description: "Una aplicación de escritorio que nos muestra información sobre el hardware y el software del equipo donde se ejecuta.",
    link: 'https://github.com/PerPab/SpecsMonitor'

},
{
    title: "Agenda de contactos en ASP",
    description: "Una agenda creada en ASP con vistas en Razor y operaciones CRUD sobre una base de datos en SQlite.",
    link: 'https://github.com/PerPab/Agenda-ASP.Net/tree/master'

},
{
    title: "Práctica con objetos",
    description: "Una aplicación de consola hecha en C# donde dos Robots se crean con stats aleatorios y combaten hasta que uno en vencido.",
    link: 'https://github.com/PerPab/Practica-Robots'

},
{
    title: "Práctica Drag & Drop",
    description: "Una aplicación realizada en Javascript, al arrastrar los objetos dentro del área, se suman o restan",
    link: 'https://drag-and-drop-practica.vercel.app/'

},
]



</script>
    
<style scoped>
p {
    user-select: none;
}

h5 {
    color: #F8F9FA;
    user-select: none;
}

.about {
    width: 100%;
    height: calc(100vh - 86px);
    overflow-y: hidden;
    overflow-x: hidden;
    background-color: #28292A;
}

.card-container {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}

.contenedor {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    
}


@media (max-width: 720px) {
    .about {
    width: 100%;
    height: calc(100vh - 86px);
    background-color: #28292A;
    overflow-y:scroll;
    overflow-x: scroll;
}

}
</style>

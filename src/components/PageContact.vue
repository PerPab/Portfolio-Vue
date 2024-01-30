<template>
    <div class="container-fluid d-flex flex-column align-items-center justify-content-start m-0 p-0 about">
        <h5 class="text-center mt-1">Contacto</h5>
        <div class="container-fluid d-flex flex-column align-items-center justify-content-start">
            <div v-for="item in info" v-bind:key="item.title" class="p-0 m-0 container-fluid">
                <CardContact :title="item.title" :description="item.description" :link="item.link" :logo="item.logo" />
            </div>

        </div>

    </div>
</template>
    
<script setup>
import CardContact from './CardContact.vue';

let info = [{
    title: "percara.pablo@gmail.com",
    link: 'mailto:percara.pablo@gmail.com',
    logo:'./img/mail.png'
},
{
    title: "pablo-percara",
    link: 'https://www.linkedin.com/in/pablo-percara/',
    logo:'./img/link.png'
},
{
    title: "PerPab",
    link: 'https://github.com/PerPab',
    logo:'./img/git.png'

},
{
    title: "Temperley - Buenos Aires",
    link: 'https://maps.app.goo.gl/Rk3dzArZj51FLg3c6',
    logo:'./img/loc.png'

}]



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



@media (max-width: 720px) {}
</style>
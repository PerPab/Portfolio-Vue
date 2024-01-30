<template>
    <div class="m-1 p-0 container-fluid d-flex flex-column justify-content-center align-items-center">
        <a v-bind:href="props.link" target="_blank" class="btn">
            <div class="container-fluid d-flex flex-row align-items-center contact-card m-2" >
                <div class="m-2">
                        <img v-bind:src="logo" class="img-fluid rounded-start logo" alt="logo">
                </div>
                <div>
                    <h6>{{ props.title }}</h6>
                </div>               
            </div>
        </a>
    </div>
</template>


<script setup>
import { defineProps } from 'vue';

const props = defineProps({
    title: String,
    link: String,
    logo:String
})
</script>


<style scoped>

.contact-card{
    width:100%;
    background-color: #F8F9FA;
    border-radius: 8px;
}
.logo{
    width: 30px;
}




a {
    text-decoration: none;
    border: none;
    text-shadow: none;
    width: 50%;
   
    
}

@media (max-width: 720px){
    a {
   
    width: 95%;
   
    
}

}


</style>
<template>
    <div class="m-1 p-0">
        <a v-bind:href="props.link" target="_blank" class="btn">
        <div class="card text-center">
            <div class="card-header m-0 p-0">
                <h5 class="card-title">{{props.title}}</h5>
            </div>
            <div class="card-body">
                <p class="card-text">{{props.description}}</p>         
            </div>
        </div>
    </a>

    </div>
</template>


<script setup>
import { defineProps } from 'vue';

const props = defineProps({
    title:String,
    description: String,
    link: String
})
</script>


<style scoped>
.card{
    width: 240px;
    min-height: 240px;
    border: none;
    
}
.card-header{
    background-color: #637A9F;
    color: #F8F9FA;
}

.card-text{
    color:#28292A;
}

a{
    text-decoration: none;
    border: none;
    text-shadow: none;
}
a:hover{
    transform: scale(1.02);
}

@media (max-width: 720px) {
    .card{
    width: 280px;
    min-height: 240px;
    border: none;
    
}
}

</style>
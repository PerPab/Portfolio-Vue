<template>
    <div class="container-fluid d-flex flex-column align-items-center justify-content-start  m-0 p-0 about">
        <h5 class="text-center mt-1">Estudios</h5>
        <div class="container container-text p-2 d-flex justify-content-center animate__animated animate__bounceIn">
            <div class="accordion open" id="accordionExample">
                <div class="accordion-item">
                    <h2 class="accordion-header" id="headingOne">
                        <button class="accordion-button" type="button" data-bs-toggle="collapse"
                            data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                            <b>Oracle Next Education</b>
                        </button>
                    </h2>
                    <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne"
                        data-bs-parent="#accordionExample">
                        <div class="accordion-body">
                            <p>Comencé mi formación gracias a una beca de Oracle llamada
                                <b>Oracle
                                    Next Education</b>.
                                El curso estuvo a cargo de Alura LATAM y durante esos meses
                                vimos un
                                amplio temario que iba desde Javascript, html y Css
                                hasta Java y SQL.
                            </p>
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header" id="headingTwo">
                        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                            data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                            <b>Auxiliar en Programación</b>
                        </button>
                    </h2>
                    <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo"
                        data-bs-parent="#accordionExample">
                        <div class="accordion-body">
                            <p>Durante el 2022 comencé la <b>Tecnicatura en Programación</b> en
                                TECLAB,
                                completando
                                el primer año de estudios y obteniendo el título intermedio de
                                Auxiliar en Programación.</p>
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header" id="headingThree">
                        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                            data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
                            <b>Desarrollo de Software</b>
                        </button>
                    </h2>
                    <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree"
                        data-bs-parent="#accordionExample">
                        <div class="accordion-body">
                            <p>En 2023 decidí cambiar de carrera a la de
                                <b>Desarrollo de Software</b> en ISTEA porque sentí que se
                                adaptaba
                                mejor a
                                mis objetivos. Aprendí C# y SQL Server y a desarrollar interfaces gráficas 
                                con WPF, y a crear aplicaciones progresivas con Javascript.
                            </p>
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header" id="heading4">
                        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                            data-bs-target="#collapse4" aria-expanded="false" aria-controls="collapse4">
                            <b>Administración de Empresas</b>
                        </button>
                    </h2>
                    <div id="collapse4" class="accordion-collapse collapse" aria-labelledby="heading4"
                        data-bs-parent="#accordionExample">
                        <div class="accordion-body">
                            <p>En 2023 también comencé la carrera de <b>Administración de Empresas
                                </b> en la UTN, con el objetivo de sumar conocimientos sobre gestión
                                que después pueda aplicar en mis programas.
                            </p>
                        </div>
                    </div>
                </div>
            </div>

        </div>
    </div>
</template>
    
<script setup></script>
    
<style scoped>
p {
    user-select: none;
    font-size: 1.2rem;
    font-weight: 100;
}

h5 {
    color: #F8F9FA;
    user-select: none;
}

.accordion-collapse {
    background-color: #F8F9FA;
}

.about {
    width: 100%;
    height: calc(100vh - 86px);
    overflow-y: hidden;
    overflow-x: hidden;
    background-color: #28292A;

}

.accordion {
    width: 70%;
    background-color: #F8F9FA;
    --bs-accordion-btn-bg: #F8F9FA;
    --bs-accordion-btn-color: #28292A;
    --bs-accordion-active-bg: #637A9F;
    --bs-accordion-active-color: #F8F9FA;
    --bs-accordion-btn-focus-box-shadow: none;
    border: #28292A solid 4px;
    border-radius: 10px;
}

.accordion-button {
    box-shadow: none;
    border: #F8F9FA 2px solid;
}

@media (max-width: 720px) {
    .accordion {
        width: 95%;
    }

    p {
    font-size: 1.1rem;
    font-weight: 400;
}

}
</style>

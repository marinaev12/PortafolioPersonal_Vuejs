<script setup>
import icono1 from '/src/assets/computer-svgrepo-com.svg';
import icono2 from '/src/assets/security-shield-svgrepo-com.svg';
import icono3 from '/src/assets/access-svgrepo-com.svg';
import icono4 from '/src/assets/cloud-computing-cloud-svgrepo-com.svg';

import { ref } from 'vue';
const titulo = 'Analista de Operaciones IT';
const fecha = 'Desde Febrero 2023 / Actualmente';
const experiencias = ref([
    { id: 1, src: icono1, parrafo: 'Responsable del área de Incidents (Portugal) en cliente global.'},
    { id: 2, src: icono2, parrafo: 'Análisis de eventos de seguridad para proteger la confidencialidad, integridad y disponibilidad de los sistemas de información de acuerdo con los objetivos del cliente, los requisitos reglamentarios y las metas estratégicas de la empresa.' },
    { id: 3, src: icono3, parrafo: 'Responsable de los procesos de Termination y Provisioning, utilizando el modelo de control de acceso basado en roles (RBAC).' },
    { id: 4, src: icono4, parrafo: 'Uso de bases de datos y aplicaciones en la nube para la seguridad de la información.' },
]);
</script>

<template>
    <div class="card">
        <h3 class="titulo">{{ titulo.toLocaleUpperCase() }}</h3>
        <p class="fecha">{{ fecha }}</p>
        <ul class="listado">
            <li class="item" v-for="experiencia in experiencias" :key="experiencia.id">
                <img class="imagen-svg" :src="experiencia.src" width="45rem" :alt="experiencia.parrafo">
                <p>{{ experiencia.parrafo }}</p>
            </li>
        </ul>
    </div>
</template>

<style scoped>
.card {
    display: flex;
    flex-direction: column;
    padding: 2rem;
    background-color: rgb(28, 41, 52);
    border-radius: 15px;
}

.titulo {
    font-size: 1.5rem;
    color: coral;
}

.fecha {
    font-size: 1rem;
    color: burlywood;
    margin-bottom: 1rem;
}

.listado {
    display: flex;
    flex-direction: column;
}

.item {
    align-items: center;
    display: flex;
    padding: 1rem;
    gap: 1.5rem;
    color: aliceblue;
}
</style>

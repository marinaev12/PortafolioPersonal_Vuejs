<script setup>
import NavBar from './components/NavBar.vue';
import DatosPersonales from './components/DatosPersonales.vue';
import Educacion from './components/EducacionPort.vue';
import ExperienciaComponente from './components/ExperienciaComponente.vue';
import ProyectosComponente from './components/ProyectosComponente.vue';
</script>

<template>
    <header>
        <!--Barra de Navegación-->
         <NavBar />
         <!--Componente Datos Personales-->
         <DatosPersonales/>
       
    </header>

    <main>
        <section id="educacion"><h2>Educación</h2></section>
        <Educacion/>
        <section id="experiencia"><h2>Experiencia</h2></section>
        <ExperienciaComponente/>
        <section id="proyectos"><h2>Proyectos</h2></section>
        <ProyectosComponente/>
        <section id="habilidades"><h2>Habilidades</h2></section>
        <section id="intereses"><h2>Intereses</h2></section> 
    </main>

</template>

<style scoped>

</style>

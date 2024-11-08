<script setup>
import NavBar from './components/NavBar.vue';
import DatosPersonales from './components/DatosPersonales.vue';
import Educacion from './components/EducacionPort.vue';
import ExperienciaComponente from './components/ExperienciaComponente.vue';
import ProyectosComponente from './components/ProyectosComponente.vue';
import HabilidadesComponente from './components/HabilidadesComponente.vue';
import InteresesComponente from './components/InteresesComponente.vue';
</script>

<template>
    <header id="top">
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
        <HabilidadesComponente/>
        <section id="intereses"><h2>Intereses</h2></section>
        <InteresesComponente/>
    </main>

<footer>
    <a href="#top">Inicio</a>
    <p>© 2024 Marina Evangelista - Portafolio Web - Tutorial UTN FRSR</p>
</footer>
</template>

<style scoped>
footer {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 2rem;
    font-size: 1.3rem;
    font-size: small;
}

footer a[href="#top"] {
    color:  rgba(30, 30, 30);
    text-decoration: none;
}

footer a[href="#top"]:hover {
    color: darkblue; /* color al pasar el mouse */
}
</style>

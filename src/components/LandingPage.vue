<template>
    <div>
    <section id="inicio">

        <h1>Vue.js 3</h1>

    </section>    
    <section id="introduccion">
      <div v-if="mostrarIntro">
        <h2>¿Que es Vue.js 3?</h2>
        <p>
            Vue es un framework de JavaScript para construir interfaces de usuario. Está diseñado para crear aplicaciones web interactivas y modernas con rapidez y facilidad. También se consolida como una de las herramientas más queridas por los ingenieros de software.
        </p>
<p>Vue 3 es la última versión de este framework, prometiendo mejoras en rendimiento, sintaxis y capacidades sin precedentes. Las novedades incluyen optimización del código, mejoras en la sintaxis y el manejo de errores, así como nuevas características como Suspense y Composition API. Esta última nos permite escribir códigos más simples, limpios y reutilizables.
        </p>
      </div>
    </section>

    <section id="historia">

        <h2>Historia</h2>
        <p>  Fue creado en 2013 por Evan You, un exingeniero de Google que quería una solución más ágil y sencilla que AngularJS.
En 2014, Vue.js se lanzó públicamente y rápidamente ganó popularidad por su sintaxis simple y su reactividad eficiente.
A lo largo de los años, Vue.js se estableció como un marco popular en el desarrollo web, siendo adoptado por empresas destacadas.
Las versiones posteriores, especialmente Vue 2 en 2016 y Vue 3 en 2020, introdujeron mejoras significativas, incluyendo mejoras de rendimiento y reescrituras del núcleo. </p>
    </section>   

  
      <section id="caracteristicas"> 
      <h2>Características de Vue.js 3</h2>
      <ul>
        <li v-for="caracteristica in caracteristicas" :key="caracteristica">
          {{ caracteristica }}
        </li>
      </ul>
    </section>

    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        mostrarIntro: true,
        caracteristicas: [
          'Es completamente modular.',
          'Tiene propiedades reactivas, si una variable cambia en una parte de la pagina, vue actualizará el nuevo valor sin necesidad de hacerlo manualmente',
          'Se basa en componentes web. Puede ser reutilizado y normalmente tiene estilos y funcionalidad aislada.',
          'Crea una replica del DOM para que al momento de hacer cambios, se hagan de forma más óptima.',
          'Se puede reaccionar a eventos que se producen en el DOM.',
          'Se tiene control sobre el ciclo de vida de los componentes, se puede controlar lo que ocurre antes, despues o durante la carga del componente.'
        ]
      };
    }
  };
  </script>
  
<style>
/* #region Sections */
section {
scroll-margin-top:  50px;
padding: 20px;
height: auto;
margin: 20px;
}

h1 {
font-size: 3rem;
color: white;
font-weight: 600;
margin-top: 50px;
padding: 50px;
     
}
h2 {
font-size: 2rem;
color: #41b883;
font-weight: 600;
}

p, li {
    font-size: 1.2rem;
}
#inicio {
    background-color: #364F6B;
    margin-left: 0;
    margin-right: 0;
}

/* #endregion */

#caracteristicas ul {
    list-style: none;
}

#caracteristicas li {
    background-color: rgba(65, 184, 131, 0.2);
    padding: 20px;
    margin: 10px;
    border-radius: 10px;
}
</style>
  
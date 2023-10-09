<template>
    <div>
    <section id="inicio">

        <h1>Vue.js 3</h1>

    </section>    
    <section id="introduccion">
      <div v-if="mostrarIntro">
        <h2>¿Que es Vue.js 3?</h2>
        <p>
          
        </p>
      </div>
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
          '',
          '',
          '',
          '',
          ''
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

#inicio {
    background-color: #34495e;
}

/* #endregion */

#caracteristicas ul {
    list-style: none;
}

#caracteristicas li {
    background-color: rgba(65, 184, 131, 0.2);
    padding: 10px;
    margin: 10px;
    border-radius: 10px;
}
</style>
  
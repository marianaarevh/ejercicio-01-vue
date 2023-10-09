<template>
    <div id="enlace">
      <h2>¿Necesitas más información?</h2>
      <p>Visita: </p> 
        <p><a :href="url">{{ url }}</a></p>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      url: {
        type: String,
        required: true
      }
    }
  };
  </script>
  
  <style>
  #enlace {
    margin: 0px;
    padding: 20px;
    background-color: #34495e;
    color: white;
  }
  #enlace h2 {
    color: white;
  }

  #enlace a{
    color: white;
    text-decoration: none;
    font-size: 1.4rem;
  }
  </style>
  
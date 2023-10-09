<template>
    <header>
        <img id="logo" src="../assets/logo.png" alt="Vue">
        <nav>
            <ul>
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#introduccion">Introduccion</a></li>
                <li><a href="#historia">Historia</a></li>
                <li><a href="#caracteristicas">Caracteristicas</a></li>
            </ul>
        </nav>
    </header>
    </template>
    
    <script>
    export default {
      name: 'MenuPrincipal',
    }
    </script>

<style>
/* #region NavBar */
header {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items:center;
  height: 60px;
  background: white;
  position: fixed;
  width: 100%;
  box-shadow: 0px 0.5px 5px 1px rgb(67, 221, 230, 0.2);
  margin-top: 0;
}


#logo {
height: 55px;
width: 55px;
margin: 20px;
display: flex;
}

#logo > img {
width: auto;
padding: 5px;
}

nav {
  display: flex;
  align-items: center;
  height: 60px;
  font-size: 1.25rem;
  box-shadow: #364F6B;
  padding: 20px;
}

nav ul {
  list-style: none;

  display: flex;
  justify-content: space-between;
}


nav li {
padding: 1rem 3rem;
}


nav li:hover a {
color: #41b883;
}

nav a {
text-decoration: none;
color: #364F6B;
font-weight: 600;
}
/* #endregion */


</style>
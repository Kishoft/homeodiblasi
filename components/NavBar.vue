<template>
<div id="top-bar">
  <figure class="logo">
    <img src="~/assets/s2.png" alt="Logo">
  </figure>
  <nav>
      <NuxtLink to="/">Inicio</NuxtLink>
      <NuxtLink to="/filosofia">Filosofía</NuxtLink>
      <NuxtLink to="/doctores">Doctores</NuxtLink>
      <NuxtLink to="/consultorios">Consultorios</NuxtLink>
      <NuxtLink to="/casos">Casos Clínicos</NuxtLink>
      <NuxtLink to="/contacto">Contacto</NuxtLink>
  </nav>
</div>
</template>

<script>
export default {

}
</script>

<style>
  #top-bar{
    display:flex;
    justify-content: space-between;
    align-items: center;
    position: sticky;
    top:0;
    background: var(--color3);
  }
  #top-bar .logo{
    margin: 0;
    padding: 0;
  }
  nav{
    display:flex;
    justify-content: center;
    align-items: center;
  }
  nav a{
    margin: 2px 4px;
    padding: 5px 10px;
    text-decoration: none;
    text-transform: uppercase;
    color: var(--color1);
    border-radius: 5px;
  }
  nav a:hover, nav a.nuxt-link-exact-active{
    background: var(--color1);
    color: var(--color3);
  }
</style>
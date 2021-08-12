<template>
<div id="top-bar" class="glass">
  <div id="top-bar-toggle-btn" :class="{ open: isOpen }" @click.prevent="toggle">
    <div class="top-bar-line"></div>
    <div class="top-bar-line"></div>
    <div class="top-bar-line"></div>
  </div>
  <figure class="logo">
    <img src="~/assets/images/s2.png" alt="Logo">
  </figure>
  <nav :style="{ left: open ? '0' : '-100%' }">
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
  data(){
    return {
      open : false
    }
  },
  computed: {
    isOpen(){
      return this.open
    }
  },
  methods: {
    toggle(){
      this.open = !this.open
    }
  }
}
</script>

<style>
  #top-bar{
    display:flex;
    width: 100%;
    justify-content: space-around;
    align-items: center;
    position: fixed;
    top:0;
    z-index: 9999;
    height: var(--nav-bar-height);
  }
  #top-bar .logo{
    margin: 0;
    padding: 0;
  }
  #top-bar nav{
    display:flex;
    justify-content: center;
    align-items: center;
    border-radius: 5px;
    background: var(--color3);
  }
  #top-bar nav a{
    margin: 2px 4px;
    padding: 5px 10px;
    text-decoration: none;
    text-transform: uppercase;
    color: var(--color1);
    border-radius: 5px;
  }
  #top-bar nav a:hover, #top-bar nav a.nuxt-link-exact-active, #top-bar nav a.nuxt-link-active{
    background: var(--color1);
    color: var(--color3);
  }
  #top-bar img {
    width: 180px;
  }
  @media (max-width: 830px) {
    #top-bar{
      justify-content: space-between;
    }
    #top-bar-toggle-btn{
      display:flex;
      flex-direction: column;
      justify-content: space-evenly;
      align-items: center;
      width: 50px;
      height: 45px;
      border: 1px solid var(--color2);
      box-sizing: border-box;
      margin: 20px;
      cursor: pointer;
    }
    #top-bar-toggle-btn .top-bar-line{
      position: relative;
      display: flex;
      width: 100%;
      height: 5px;
      background: var(--color2);
    }
    #top-bar nav{
      flex-direction: column;
      position: fixed;
      transition: all .3s ease-in-out;
      top: var(--nav-bar-height);
      width: 80%;
    }
  }
</style>
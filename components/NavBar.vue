<template>
<div id="top-bar" class="glass">
  <figure class="logo">
    <img src="~/assets/images/s2.png" alt="Logo">
  </figure>
  <div id="top-bar-toggle-btn" @click.prevent="toggle">
    <div :style="{ transform : open ? 'rotate(37deg) translateX(5px)' : 'rotate(0deg)' }" class="top-bar-line"></div>
    <div :style="{ opacity : open ? 0 : 1 }" class="top-bar-line"></div>
    <div :style="{ transform : open ? 'rotate(-37deg) translateX(5px)' : 'rotate(0deg)' }" class="top-bar-line"></div>
  </div>
  <nav :style="{ left: open ? '0' : '-100%' }">
      <NuxtLink to="/filosofia" @click.native="close">Filosofía</NuxtLink>
      <NuxtLink to="/doctores" @click.native="close">Doctores</NuxtLink>
      <NuxtLink to="/casos" @click.native="close">Casos Clínicos</NuxtLink>
      <NuxtLink to="/contacto" @click.native="close">Contacto</NuxtLink>
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
    },
    close(){
      this.open = false;
    }
  }
}
</script>

<style>
  #top-bar{
    display:flex;
    width: 100%;
    justify-content: space-evenly;
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
    border-radius: 5px;
    color: var(--color1);
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
      justify-content: space-between;
      align-items: center;
      width: 50px;
      height: 45px;
      border: 1px solid var(--color2);
      box-sizing: border-box;
      margin: 20px;
      cursor: pointer;
      border-radius: 5px;
      padding: 5px;
    }
    #top-bar-toggle-btn .top-bar-line{
      position: relative;
      display: flex;
      width: 100%;
      height: 5px;
      transform-origin: left;
      transition: all .5s ease;
      border-radius: 5px;
      background: var(--color2);
    }
    #top-bar nav{
      flex-direction: column;
      position: fixed;
      transition: all .3s ease-in-out;
      top: var(--nav-bar-height);
      width: 100%;
    }
  }
</style>
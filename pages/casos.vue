<template>
    <div id="content">
        <header>
            <h2 class="glass">Casos Clínicos</h2>
        </header>
        <main class="glass">
            <SideNav/>
            <NuxtChild/>
        </main>
    </div>
</template>

<script>
import SideNav from '~/components/SideNav.vue';
export default {
  components : { SideNav },
  middleware({ route, redirect}){
    if(route.name === 'casos') redirect('/casos/clinicos')
  }
}
</script>

<style scoped>
  #content{
    background: url('~/assets/images/header4.jpg');
    background-attachment: fixed;
    background-position: center center;
    background-size: cover;
    background-repeat: no-repeat;
    box-sizing: border-box;
  }

  main{
      display:grid;
      grid-template-columns: var(--side-bar-width) auto;
    }

  @media (max-width: 830px) {
    main{
      grid-template-columns: auto;
      grid-template-rows: auto auto;
    }
  }
</style>
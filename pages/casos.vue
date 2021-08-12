<template>
    <div id="content">
        <header>
            <h2>Casos Clínicos</h2>
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
  }
  main{
    display:grid;
    grid-template-columns: var(--side-bar-width) auto;
  }
</style>
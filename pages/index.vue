<template>
    <div id="content">
        <header>
            <h2>Homeopatía Unicista</h2>
        </header>
    </div>
</template>

<script>
export default {
  middleware({ route, redirect}){
    if(route.name === 'index') redirect('/filosofia/que_es')
  }
}
</script>
<style scoped>
  #content{
    background: url('~/assets/images/header1.jpg');
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

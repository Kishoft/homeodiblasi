<template>
  <div>
    <header>
      <h1>Doctores</h1>
    </header>
    <NuxtLink to="/doctores/maria">
        <h4 class="doctor">Doctora María Laura Diblasi</h4>
    </NuxtLink>
    <NuxtLink to="/doctores/lucia">
        <h4 class="doctor">Doctora Lucía Diblasi</h4>
    </NuxtLink>
    <NuxtLink to="/doctores/jose">
        <h4 class="doctor">Doctor José Diblasi</h4>
    </NuxtLink>  
    <NuxtChild/>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
  header{
    background: url('~/assets/header2.jpg');
    background-attachment: fixed;
    background-position: center center;
    background-size: cover;
    background-repeat: no-repeat;
  }
</style>
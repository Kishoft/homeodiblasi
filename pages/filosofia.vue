<template>
    <div>
        <header>
            <h1>Homeopatía Unicista</h1>
        </header>
        <SideNav/>
        <NuxtChild/>
    </div>
</template>

<script>
import SideNav from '~/components/filosofia/SideNav.vue';
export default {
  components : { SideNav }
}
</script>
<style scoped>
  header{
    background: url('~/assets/header1.jpg');
    background-attachment: fixed;
    background-position: center center;
    background-size: cover;
    background-repeat: no-repeat;
  }
</style>

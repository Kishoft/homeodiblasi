<template>
    <div>
        <header>
            <h1>Casos Clínicos</h1>
        </header>
        <SideNav/>
        <NuxtChild/>
    </div>
</template>

<script>
import SideNav from '~/components/casos/SideNav.vue';
export default {
  components : { SideNav }
}
</script>

<style>

</style>
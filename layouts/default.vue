<template>
<div>
    <NavBar/>
    <Nuxt />
    <Footer/>
</div>
</template>

<script>

export default {
  
}
</script>

<style>
  :root{
    --color1: #638733;
    --color2: #4A7324;
    --color3: white;
  }
  html, body{
    margin: 0;
    padding: 0;
    font-family: 'Segoe UI', Tahoma, Verdana, Arial, Helvetica, sans-serif;
  }
  header{
    display:flex;
    justify-content: space-evenly;
    align-items: center;
    height: 35vh;
    max-height: 900px;
  }
  h1{
    color: var(--color3)
  }
</style>
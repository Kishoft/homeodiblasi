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
    --nav-bar-height: 120px;
    --side-bar-width: 250px;
  }
  @media (max-width: 830px) {
    :root{
      --nav-bar-height: 80px;
    }
    section img{
      max-width: 120px;
    }
  }
  html, body{
    margin: 0;
    padding: 0;
    font-family: 'Segoe UI', Tahoma, Verdana, Arial, Helvetica, sans-serif;
    scroll-behavior: smooth;
    scroll-padding-top: var(--nav-bar-height);
  }
  body, #content{
    min-height: 100vh;
  }
  main{
    box-sizing: border-box;
    max-width: 1200px;
    margin: auto;
    border-radius: 10px;
  }
  main > section {
    border-radius: 5px;
    padding: 5px 10px;
  }
  header{
    display:flex;
    justify-content: space-evenly;
    align-items: center;
    height: 20vh;
    max-height: 900px;
    padding-top: var(--nav-bar-height);
  }
  h2{
    padding: 5px 10px;
    border-radius: 15px;
    color: var(--color2);
  }
  section img{
    float:right;
    margin: 10px;
  }
  .glass{
    background: rgba( 255, 255, 255, 0.6 );
    box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
    backdrop-filter: blur( 15px );
    -webkit-backdrop-filter: blur( 15px );
    border: 1px solid rgba( 255, 255, 255, 0.4 );
  }
</style>
<template>
  <div id="content">
    <header>
      <h2>Doctores</h2>
    </header>
    <main class="glass">
      <section id="cards">
        <figure class="glass">
          <figcaption>
            <h4 class="doctor">Doctora María Laura Diblasi</h4>
            <NuxtLink to="/doctores/maria">Conocer</NuxtLink>
          </figcaption>
        </figure>
        <figure class="glass">
          <figcaption>
            <h4 class="doctor">Doctora Lucía Diblasi</h4>
            <NuxtLink to="/doctores/lucia">Conocer</NuxtLink>
          </figcaption>
        </figure>
        <figure class="glass">
          <figcaption>
            <h4 class="doctor">Doctor José Diblasi</h4>
            <NuxtLink to="/doctores/jose">Conocer</NuxtLink>  
          </figcaption>
        </figure>
      </section>
      <section>
        <NuxtChild/>
      </section>
    </main>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
  #content{
    background: url('~/assets/images/header3.jpg');
    background-attachment: fixed;
    background-position: center center;
    background-size: cover;
    background-repeat: no-repeat;
  }
  #cards{
    display:flex;
    justify-content: space-evenly;
    align-items: flex-start;
  }
  figure{
    padding: 0 10px;
  }
  figcaption{
    display:flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }
  #cards a{
    margin: 2px 4px 10px 4px;
    padding: 5px 10px;
    text-decoration: none;
    text-transform: uppercase;
    border-radius: 5px;
    color: var(--color3);
    background: var(--color2);
  }
</style>
<template>
  <div id="content">
    <header>
      <h2 class="glass">Doctores</h2>
    </header>
    <main class="glass">
      <section id="cards">
        <figure class="glass">
          <figcaption>
            <h4 class="doctor">Doctora María Laura Diblasi</h4>
            <h5>(M.N. :113276 - MP:332507)</h5>
            <img src="~/assets/images/pages/dra_maria_laura_diblasi.jpg" alt="">
            <NuxtLink @click.native="scrollToHeader" to="/doctores/maria_laura_diblasi/informacion_personal">Información Personal</NuxtLink>
            <NuxtLink @click.native="scrollToHeader" to="/doctores/maria_laura_diblasi/educacion">Educación</NuxtLink>
            <NuxtLink @click.native="scrollToHeader" to="/doctores/maria_laura_diblasi/actividades_academicas">Actividades Académicas</NuxtLink>
            <NuxtLink @click.native="scrollToHeader" to="/doctores/maria_laura_diblasi/seminarios_y_cursos">Seminarios y Cursos</NuxtLink>
            <NuxtLink @click.native="scrollToHeader" to="/doctores/maria_laura_diblasi/publicaciones">Publicaciones</NuxtLink>
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
  methods : {
    scrollToHeader(){
      console.log("Beep")
      console.log(document.querySelector("h3"))
      document.querySelector("h3").scrollIntoView()
    }
  }
}
</script>

<style scoped>
  #content{
    background: url('~/assets/images/header3.jpg');
    background-attachment: fixed;
    background-position: center center;
    background-size: cover;
    background-repeat: no-repeat;
    box-sizing: border-box;
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
    border: 1px solid var(--color2);
    color: var(--color3);
    background: var(--color2);
  }
  #cards a.nuxt-link-exact-active{
    color: var(--color2);
    background: var(--color3);
  }
</style>
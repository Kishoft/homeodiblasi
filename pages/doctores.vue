<template>
  <div id="content">
    <header>
      <h2 class="glass">Doctores</h2>
    </header>
    <main class="glass">
      <section id="cards">
        <figure class="glass">
          <figcaption>
            <h3 class="doctor">Doctora María Laura Diblasi</h3>
            <h5>(M.N. : 113276 - M.P. : 332507)</h5>
            <img src="~/assets/images/pages/dra_maria_laura_diblasi.jpg" alt="">
            <NuxtLink @click.native="scrollToHeader" to="/doctores/maria_laura_diblasi/informacion_personal">Información Personal</NuxtLink>
            <NuxtLink @click.native="scrollToHeader" to="/doctores/maria_laura_diblasi/educacion">Educación</NuxtLink>
            <NuxtLink @click.native="scrollToHeader" to="/doctores/maria_laura_diblasi/actividades_academicas">Actividades Académicas</NuxtLink>
            <NuxtLink @click.native="scrollToHeader" to="/doctores/maria_laura_diblasi/seminarios_y_cursos">Seminarios y Cursos</NuxtLink>
            <NuxtLink @click.native="scrollToHeader" to="/doctores/maria_laura_diblasi/publicaciones">Publicaciones</NuxtLink>
          </figcaption>
        </figure>
        <figure class="glass">
          <figcaption>
            <h3 class="doctor">Doctora Luciana Diblasi</h3>
            <h5>(M.N. : 119849 - M.P.: 333840)</h5>
            <img src="~/assets/images/pages/dra_luciana_diblasi.jpg" alt="">
            <NuxtLink @click.native="scrollToHeader" to="/doctores/luciana_diblasi/informacion_personal">Información Personal</NuxtLink>
            <NuxtLink @click.native="scrollToHeader" to="/doctores/luciana_diblasi/educacion">Educación</NuxtLink>
            <NuxtLink @click.native="scrollToHeader" to="/doctores/luciana_diblasi/seminarios_y_cursos">Seminarios y Cursos</NuxtLink>
            <NuxtLink @click.native="scrollToHeader" to="/doctores/luciana_diblasi/publicaciones">Publicaciones</NuxtLink>
          </figcaption>
        </figure>
        <figure class="glass">
          <figcaption>
            <h3 class="doctor">Doctor José Diblasi</h3>
            <h5>(M.N. : 62663 - M.P. : 35493)</h5>
            <img src="~/assets/images/pages/dra_luciana_diblasi_2.jpg" alt="">
            <NuxtLink @click.native="scrollToHeader" to="/doctores/jose_diblasi/informacion_personal">Información Personal</NuxtLink>
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
      document.querySelector("h4").scrollIntoView()
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
    flex-wrap: wrap;
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
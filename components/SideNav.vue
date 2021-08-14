<template>
  <aside :style="{ left: open ? '0' : '-100%' }">
    <div id="aside-toggle-btn" class="glass" @click.prevent="toggle">
      <div :style="{ transform : open ? 'rotate(37deg) translateX(5px)' : 'rotate(22deg)' }" class="aside-line"></div>
      <div :style="{ transform : open ? 'rotate(-37deg) translateX(5px)' : 'rotate(-22deg)' }" class="aside-line"></div>
    </div>
    <nav v-if="$nuxt.$route.name.includes('casos')">
      <NuxtLink to="/casos/gastritis_cronica" @click.native="close">Gastritis Crónica</NuxtLink>
      <NuxtLink to="/casos/rinitis_alergica" @click.native="close">Rinitis Alérgica</NuxtLink>
      <NuxtLink to="/casos/migrania" @click.native="close">Migraña</NuxtLink>
      <NuxtLink to="/casos/infeccion_urinaria" @click.native="close">Infección Urinaria</NuxtLink>
      <NuxtLink to="/casos/sindrome_reynaud" @click.native="close">Síndrome de Reynaud<br />(insuficiencia vascular)</NuxtLink>
      <NuxtLink to="/casos/dishidrosis" @click.native="close">Dishidrosis</NuxtLink>
      <NuxtLink to="/casos/asma" @click.native="close">Niña con Asma</NuxtLink>
      <NuxtLink to="/casos/sinusitis_cronica" @click.native="close">Sinusitis Crónica</NuxtLink>
      <NuxtLink to="/casos/hiperplasia_prostata" @click.native="close">Hiperplasia de Próstata</NuxtLink>
      <NuxtLink to="/casos/dismenorrea" @click.native="close">Dismenorrea y Alteraciones menstruales</NuxtLink>
      <NuxtLink to="/casos/depresion" @click.native="close">Depresión</NuxtLink>
      <NuxtLink to="/casos/varices" @click.native="close">Varices y Gastritis Crónica</NuxtLink>
      <NuxtLink to="/casos/sobrepeso" @click.native="close">Sobrepeso</NuxtLink>
      <NuxtLink to="/casos/panico" @click.native="close">Ataque de Pánico</NuxtLink>
      <NuxtLink to="/casos/verrugas" @click.native="close">Un niño con Verrugas</NuxtLink>
      <NuxtLink to="/casos/hiperemesis" @click.native="close">Hiperémesis Gravídica</NuxtLink>
      <NuxtLink to="/casos/hiperqueratosis" @click.native="close">Hiperqueratosis Plantar</NuxtLink>
      <NuxtLink to="/casos/ezquizofrenia" @click.native="close">Un Joven Esquizofrénico</NuxtLink>
      <NuxtLink to="/casos/menopausia" @click.native="close">Una Mujer Menopáusica</NuxtLink>
      <NuxtLink to="/casos/artrosis" @click.native="close">Artrosis y tromboflebitis</NuxtLink>
      <NuxtLink to="/casos/colon" @click.native="close">Colon irritable y Hemorroides</NuxtLink>
      <NuxtLink to="/casos/eccema" @click.native="close">Eccema</NuxtLink>
      <NuxtLink to="/casos/depresion_grave" @click.native="close">Depresion Grave</NuxtLink>
      <NuxtLink to="/casos/aftas_a_repeticion" @click.native="close">Aftas</NuxtLink>
      <NuxtLink to="/casos/hiperquinesia" @click.native="close">Hiperquinesia</NuxtLink>
      <NuxtLink to="/casos/bronquiolitis" @click.native="close">Bronquiolitis</NuxtLink>
      <NuxtLink to="/casos/fibromialgia" @click.native="close">Fibromialgia</NuxtLink>
      <NuxtLink to="/casos/colicos" @click.native="close">Cólicos Renales</NuxtLink>
      <NuxtLink to="/casos/psoriasis" @click.native="close">Psoriasis</NuxtLink>
      <NuxtLink to="/casos/tos" @click.native="close">Tos Cronica</NuxtLink>
      <NuxtLink to="/casos/herpes" @click.native="close">Herpes Genital</NuxtLink>
    </nav>
    <nav v-if="$nuxt.$route.name.includes('filosofia')">
      <NuxtLink to="/filosofia/que_es" @click.native="close">¿Qué es?</NuxtLink>
      <NuxtLink to="/filosofia/cuando_nace" @click.native="close">¿Cuándo nace?</NuxtLink>
      <NuxtLink to="/filosofia/como_actua" @click.native="close">¿Cómo actúa?</NuxtLink>
      <NuxtLink to="/filosofia/tratamiento_homeopatico_alopatico" @click.native="close">¿Qué diferencia hay entre el tratamiento Homeopático y el Alopático?</NuxtLink>
      <NuxtLink to="/filosofia/consulta_homeopatia" @click.native="close">¿Cómo es una consulta con un Médico Homeópata?</NuxtLink>
      <NuxtLink to="/filosofia/enfermedad" @click.native="close">Enfermedad ¿es sinónimo de enfermo?</NuxtLink>
      <NuxtLink to="/filosofia/especialidad_medica" @click.native="close">¿Por qué no está reconocida la Homeopatía como especialidad Médica?</NuxtLink>
      <NuxtLink to="/filosofia/ciencia" @click.native="close">La Homeopatía, ¿es científica?</NuxtLink>
      <NuxtLink to="/filosofia/que_cura" @click.native="close">¿Qué enfermedades puede curar la Homeopatía?</NuxtLink>
    </nav>
  </aside>
</template>

<script>
export default {
  data(){
    return {
      open : false
    }
  },
  computed: {
    isOpen(){
      return this.open
    }
  },
  methods: {
    toggle(){
      this.open = !this.open
    },
    close(){
      this.open = false;
    }
  }
}
</script>

<style>
  aside {
    background: var(--color3);
    border-radius: 10px;
  }
  aside nav{
    display:flex;
    position: static;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    height: 100%;
  }

  aside nav a{
    text-decoration: none;
    color: var(--color2);
    margin: 2px;
    padding: 5px;
    border-radius: 5px;
  }

  aside nav a:hover{
    text-decoration: underline;
  }

  #aside-toggle-btn{
    display:none;
  }

  @media (max-width: 830px) {
    aside{
      position: fixed;
      top: 0;
      width: 100%;
      transition: left .3s ease-in-out;
      max-height: calc(100vh - 20vh - var(--nav-bar-height) - 2px);
      overflow-y: scroll;
      box-sizing: border-box;
    }
    #aside-toggle-btn{
      display:flex;
      flex-direction: column;
      justify-content: space-between;
      align-items: center;
      width: 50px;
      height: 45px;
      border: 1px solid var(--color2);
      box-sizing: border-box;
      cursor: pointer;
      border-radius: 5px;
      padding: 5px;
      position: fixed;
      top: -50px;
      left: 5px;
      z-index: 9999;
    }

    #aside-toggle-btn .aside-line{
      display: flex;
      width: 100%;
      height: 5px;
      background: var(--color2);
      transform-origin: left;
      border-radius: 5px;
      transition: all .5s ease;
    }

  }
</style>
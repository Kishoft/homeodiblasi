<template>
  <aside>
    <nav v-if="$nuxt.$route.name.includes('casos')">
      <NuxtLink to="/casos/gastritis_cronica">Gastritis Crónica</NuxtLink>
      <NuxtLink to="/casos/rinitis_alergica">Rinitis Alérgica</NuxtLink>
      <NuxtLink to="/casos/migrania">Migraña</NuxtLink>
      <NuxtLink to="/casos/infeccion_urinaria">Infección Urinaria</NuxtLink>
      <NuxtLink to="/casos/sindrome_reynaud">Síndrome de Reynaud<br />(insuficiencia vascular)</NuxtLink>
      <NuxtLink to="/casos/dishidrosis">Dishidrosis</NuxtLink>
      <NuxtLink to="/casos/asma">Niña con Asma</NuxtLink>
      <NuxtLink to="/casos/sinusitis_cronica">Sinusitis Crónica</NuxtLink>
      <NuxtLink to="/casos/hiperplasia_prostata">Hiperplasia de Próstata</NuxtLink>
      <NuxtLink to="/casos/dismenorrea">Dismenorrea y Alteraciones menstruales</NuxtLink>
      <NuxtLink to="/casos/depresion">Depresión</NuxtLink>
      <NuxtLink to="/casos/varices">Varices y Gastritis Crónica</NuxtLink>
      <NuxtLink to="/casos/sobrepeso">Sobrepeso</NuxtLink>
      <NuxtLink to="/casos/panico">Ataque de Pánico</NuxtLink>
      <NuxtLink to="/casos/verrugas">Un niño con Verrugas</NuxtLink>
      <NuxtLink to="/casos/hiperemesis">Hiperémesis Gravídica</NuxtLink>
      <NuxtLink to="/casos/hiperqueratosis">Hiperqueratosis Plantar</NuxtLink>
      <NuxtLink to="/casos/ezquizofrenia">Un Joven Esquizofrénico</NuxtLink>
      <NuxtLink to="/casos/menopausia">Una Mujer Menopáusica</NuxtLink>
      <NuxtLink to="/casos/artrosis">Artrosis y tromboflebitis</NuxtLink>
      <NuxtLink to="/casos/colon">Colon irritable y Hemorroides</NuxtLink>
      <NuxtLink to="/casos/eccema">Eccema</NuxtLink>
      <NuxtLink to="/casos/depresion_grave">Depresion Grave</NuxtLink>
      <NuxtLink to="/casos/aftas_a_repeticion">Aftas</NuxtLink>
      <NuxtLink to="/casos/hiperquinesia">Hiperquinesia</NuxtLink>
      <NuxtLink to="/casos/bronquiolitis">Bronquiolitis</NuxtLink>
      <NuxtLink to="/casos/fibromialgia">Fibromialgia</NuxtLink>
      <NuxtLink to="/casos/colicos">Cólicos Renales</NuxtLink>
      <NuxtLink to="/casos/psoriasis">Psoriasis</NuxtLink>
      <NuxtLink to="/casos/tos">Tos Cronica</NuxtLink>
      <NuxtLink to="/casos/herpes">Herpes Genital</NuxtLink>
    </nav>
    <nav v-if="$nuxt.$route.name.includes('filosofia')">
      <NuxtLink to="/filosofia/que_es">¿Qué es?</NuxtLink>
      <NuxtLink to="/filosofia/cuando_nace">¿Cuándo nace?</NuxtLink>
      <NuxtLink to="/filosofia/como_actua">¿Cómo actúa?</NuxtLink>
      <NuxtLink to="/filosofia/tratamiento_homeopatico_alopatico">¿Qué diferencia hay entre el tratamiento Homeopático y el Alopático?</NuxtLink>
      <NuxtLink to="/filosofia/consulta_homeopatia">¿Cómo es una consulta con un Médico Homeópata?</NuxtLink>
      <NuxtLink to="/filosofia/enfermedad">Enfermedad ¿es sinónimo de enfermo?</NuxtLink>
      <NuxtLink to="/filosofia/especialidad_medica">¿Por qué no está reconocida la Homeopatía como especialidad Médica?</NuxtLink>
      <NuxtLink to="/filosofia/ciencia">La Homeopatía, ¿es científica?</NuxtLink>
      <NuxtLink to="/filosofia/que_cura">¿Qué enfermedades puede curar la Homeopatía?</NuxtLink>
    </nav>
  </aside>
</template>

<script>
export default {

}
</script>

<style>
  aside nav{
    display:flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    background: var(--color3);
    height: 100%;
    border-radius: 5px;
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
</style>
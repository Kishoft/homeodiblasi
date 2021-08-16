<template>
    <div id="content">
        <header>
            <h2 class="glass">Consultorios</h2>
        </header>
        <main class="glass">
            <section>
                <section id="consultorios">
                    <figure class="consultorio glass">
                        <h3>Buenos Aires - Morón</h3>
                        <dl>
                            <dt>Atienden</dt>
                            <dd>
                                <ul>
                                    <li>Dr José Di Blasi (adultos)</li>
                                    <li>Dra Luciana Di Blasi (pediatra)</li>
                                </ul>
                            </dd>
                            <dt>Dirección</dt>
                            <dd>Casullo 306, 1 B. Esquina Buen Viaje, Morón</dd>
                            <dt>Teléfono</dt>
                            <dd><a href="tel:+60890957">11-6089-0957</a></dd>
                            <dt>Whatsapp</dt>
                            <dd><a href="https://api.whatsapp.com/send?phone=+1141415693&text=Hola.%20%C2%A1Buen%20d%C3%ADa!%20Quiero%20solicitar%20un%20turno%20online">11-4141-5693</a></dd>
                            <dt>Consultas por Email</dt>
                            <dd><a href="mailto:lulydiblasi@hotmail.com">lulydiblasi@hotmail.com</a></dd>
                        </dl>
                        <h3>Mapa</h3>
                        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3282.1070615727144!2d-58.625865425869385!3d-34.65199904391601!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x95bcc75e0bfae6a9%3A0x42831a47fa5662b8!2sIPH%2C%20Dr.%20Jos%C3%A9%20Mar%C3%ADa%20Casullo%20306%2C%20B1708%20Mor%C3%B3n%2C%20Provincia%20de%20Buenos%20Aires!5e0!3m2!1ses-419!2sar!4v1628906963364!5m2!1ses-419!2sar" height="400" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
                    </figure>
                    <figure class="consultorio glass">
                        <h3>Córdoba</h3>
                        <dl>
                            <dt>Atiende</dt>
                            <dd>
                                <ul>
                                    <li><NuxtLink to="/doctores/maria_laura_diblasi/informacion_personal">Dra María Laura Di Blasi</NuxtLink></li>
                                </ul>
                            </dd>
                            <dt>Dirección</dt>
                            <dd>Av. Maganolias 456, Local 1, Villa Gral.Belgrano</dd>
                            <dt>Teléfono</dt>
                            <dd><a href="tel:+3546431504">3546 431504</a></dd>
                            <dt>Consultas por Email</dt>
                            <dd><a href="mailto:mlauradiblasi@hotmail.com">mlauradiblasi@hotmail.com</a></dd>
                        </dl>
                        <h3>Mapa</h3>
                        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3384.643074921891!2d-64.54785704868657!3d-31.970578430383803!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x95d2b0399712a7af%3A0xa6b0f46ed5934029!2sLas%20Magnolias%20456%2C%20X5194%20Villa%20Gral.%20Belgrano%2C%20C%C3%B3rdoba!5e0!3m2!1ses-419!2sar!4v1628907382230!5m2!1ses-419!2sar" height="400" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
                    </figure>
                </section>
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
    background: url('~/assets/images/header2.jpg');
    background-attachment: fixed;
    background-position: center center;
    background-size: cover;
    background-repeat: no-repeat;
    box-sizing: border-box;
  }
  
  #consultorios, #formulario{
      display:flex;
      justify-content: space-evenly;
      align-items: flex-start;
      flex-wrap: wrap;
  }

  .consultorio{
      display:flex;
      justify-content: space-evenly;
      align-items: center;
      flex-direction: column;
      flex-wrap: wrap;
      padding: 5px 20px;
      border-radius: 10px;
  }
</style>
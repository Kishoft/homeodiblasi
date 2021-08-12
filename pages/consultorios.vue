<template>
    <div id="content">
        <header>
            <h2>Consultorios</h2>
        </header>
        <main>
            <section>
	            <p>Para solicitar turno con la Doctora María Laura Di Blasi, comuníquese con alguno de los consultorios:</p>
                <div class="consultorio">
                    <h3>Morón</h3>
                    <dl>
                        <dt>Dirección</dt>
                        <dd>Casullo 457</dd>
                        <dt>Teléfono</dt>
                        <dd><a href="tel:46291714">4629-1714</a></dd>
                        <dd></dd>
                    </dl>
                </div>
                <div class="consultorio">
                    <h3>CABA</h3>
                    <dl>
                        <dt>Dirección</dt>
                        <dd>Callao 322 - 9ºD</dd>
                        <dt>Teléfono</dt>
                        <dd><a href="tel:43730180">4373-0180</a></dd>
                        <dd><a href="tel:43716199">4371-6199</a></dd>
                        <dd></dd>
                    </dl>
                </div>
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
  }
  
  main{
    display:grid;
    grid-template-columns: var(--side-bar-width) auto;
  }
</style>
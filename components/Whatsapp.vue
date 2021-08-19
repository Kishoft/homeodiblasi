<template>
  <div id="whatsapp">
      <div id="whatsappContent" class="glass" :style="{ transform: open ? 'translate(0px) skew(0deg)' : 'translate(-300px, 200px) skew(-20deg)' }">
          <p>Para solicitar turnos por Whatsapp, por favor envíe un <strong>mensaje</strong> al siguiente número.</p>
          <p>La atención virtual se ofrece de forma <strong>internacional</strong>.</p>
          <p>Las <strong>llamadas</strong> se reservan <strong>exclusivamente</strong> para sesiones con pacientes.</p>
          <a href="https://api.whatsapp.com/send?phone=+1155656130&text=Hola.%20%C2%A1Buen%20d%C3%ADa!%20Quiero%20solicitar%20un%20turno%20online">11-5565-6130</a>
      </div>
      <div id="whatsappLegend">Solicitar<br>Turno</div>
      <div id="whatsappBtn" @click="toggle"></div>
  </div>
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
    #whatsapp{
        position: fixed;
        bottom: 0;
        left: 0;
    }
    #whatsappBtn{
        position: relative;
        width: 80px;
        height: 80px;
        background: url('~/assets/images/whatsapp.png');
        background-position: center;
        background-size: 80px;
        cursor: pointer;
    }
    #whatsappLegend{
        margin-left: 10px;
        font-weight: bolder;
        text-transform: uppercase;
        color: var(--color3);
        text-shadow: 0px 0px 10px black;
    }
    #whatsappContent{
        display:flex;
        justify-content: center;
        align-items: flex-start;
        flex-wrap: wrap;
        box-sizing: border-box;
        margin-left: 10px;
        margin-bottom: 10px;
        padding: 10px;
        border-radius: 5px;
        max-width: 200px;
        transition: all .5s ease;
    }
</style>
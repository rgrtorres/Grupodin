<template>
  <div class="company">
    <div class="container d-flex align-items-center" id="company">
      <div>
        <h1>DIN LOG Transportes</h1>
        <h3>TRANSPORTADORA RODOVIÁRIA DE CARGAS.</h3>
        <p>
          A Transportadora DIN LOG conta com mais de 30 anos de expertise em
          transporte rodoviário de cargas em contêiners e fracionadas nas
          importações e exportações com orígem e/ou destino ao Porto de Santos
        </p>

        <p>
          Dispomos de um terminal com 3000 m² localizado na Margem Direita do
          Porto de Santos com oficina para manutenção de veículos. Trabalhamos
          com veículos próprios e de terceiros. Nossa frota é rastreada e
          monitorada via satélite por empresa especializada.
        </p>

        <p>Oferecemos garantia de qualidade ISO 9001 e SASSMAQ.</p>

        <p>Conheça os nossos diferenciais.</p>
      </div>

      <img
        src="http://grupodin.com.br/images/caminhao-gruposin.png"
        alt="caminhão"
        v-if="this.SizeScreen > 600"
      />
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    SizeScreen: ""
  }),
  mounted: function() {
    this.SizeScreen = window.screen.width;
    console.log(this.SizeScreen)
  }
}
</script>

<template>
  <footer class="" style="background-color: rgba(0, 0, 0, 0.1)">
    <div class="container">
      <div class="container d-flex justify-content-center">
        <img
          src="images/selo-sassmaq.png"
          alt=""
          style="margin: 0 5px"
        />
        <img
          src="images/selo-dqs.png"
          alt=""
          style="margin: 0 5px"
        />
      </div>
      <div class="text-center">
        Grupo Din © 2015 ~ {{ currentYear }} - Todos os direitos reservados
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data: () => ({
    currentYear: "",
  }),
  mounted: function () {
    this.currentYear = new Date().getFullYear();
  },
};
</script>

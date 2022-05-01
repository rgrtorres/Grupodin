<template>
  <div class="container" id="home">
    <b-navbar toggleable="lg justify-content-between align-items-center">
      <b-navbar-brand href="#">
        <img src="images/logo.png" height="65" alt="">
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="mx-auto">
          <b-nav-item href="#home">Início</b-nav-item>
          <b-nav-item href="#company">O Grupo</b-nav-item>
          <b-nav-item href="#contact">Contato</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  data: () => ({
    itemMenu: "menu",
  }),
  mounted: function () {
    console.log(this.itemMenu);
  },
};
</script>

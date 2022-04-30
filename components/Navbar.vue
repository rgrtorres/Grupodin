<template>
  <div class="container" id="home">
    <b-navbar toggleable="lg justify-content-center align-items-center">
      <b-navbar-brand href="#">Grupodin</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="menu nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#home">Início</b-nav-item>
          <b-nav-item href="#company">O Grupo</b-nav-item>
          <b-nav-item href="#contact">Contato</b-nav-item>
        </b-navbar-nav>

        <!-- <b-navbar-nav class="ml-auto">
          <b-nav-form>
            <b-form-input class="mr-sm-2" placeholder="Search"></b-form-input>
            <b-button class="my-2 my-sm-0" type="submit">Search</b-button>
          </b-nav-form>

          <b-nav-item-dropdown text="Lang" right>
            <b-dropdown-item href="#">EN</b-dropdown-item>
            <b-dropdown-item href="#">ES</b-dropdown-item>
            <b-dropdown-item href="#">RU</b-dropdown-item>
            <b-dropdown-item href="#">FA</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown right>
            <template #button-content>
              <em v-if="user">Bem vindo, {{ user.name }}!</em>
              <em v-else>Fazer login</em>
            </template>
            <b-dropdown-item href="#">Profile</b-dropdown-item>
            <b-dropdown-item @click="logout" href="#">Sign Out</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav> -->
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
// export default {
//   data() {
//     return {
//       user: null
//     }
//   },
//   mounted() {
//     this.getUserData();
//   },

//   methods: {
//     async getUserData() {
//       const { data: response } = await this.$axios.get('https://api.github.com/users/luscas');

//       this.user = response;
//     },

//     logout() {
//       this.user = null;
//       return false;
//     }
//   }
// }

export default {
  data: () => ({
    itemMenu: "menu",
  }),
  mounted: function () {
    console.log(this.itemMenu);
  },
};
</script>

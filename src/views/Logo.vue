<template>
  <v-app>
    <v-navigation-drawer v-model="drawer" absolute temporary>
      <Menu />
    </v-navigation-drawer>
    <v-container class="pa-0">
          <div class="content py-10">
            <Sidebar @accion="mostrar" />
            <v-row>
              <v-col class="content-col-1" cols="12" md="6">
                <h2>Usage Rules</h2>
                <br />
                <br />
                <p>
                  Use this logo for non-marketing related communications such as
                  fi nancial documents, building signage, letterheads, business
                  cards, etc. Maintaining clear space around the logo ensures
                  its readability:
                  <br /><br />
                  As shown, full height of the letter ‘A’ is the standard
                  measurement for calculating the clear space around the
                  stand-alone logo. Only the white or red logo may be used.
                  Download the Avaya logos in .jpeg, .eps, .gif formats here
                </p>
              </v-col>
              <v-col
                class="content-col-2 d-flex justify-center align-center"
                cols="12"
                md="6"
              >
                <img src="../img/avaya-logo.png" alt="" />
              </v-col>
            </v-row>
            <br /><br />
            <v-row class="row-all">
              <figure>
                <img src="../img/logo-colors.png" alt="" />
              </figure>
            </v-row>
          </div>
    </v-container>
  </v-app>
</template>

<script>
// @ is an alias to /src
import Menu from "../components/Menu";
import Sidebar from "../components/Sidebar";

export default {
  name: "Home",
  data() {
    return {
      drawer: null,
    };
  },
  components: {
    Menu,
    Sidebar,
  },
  methods: {
    mostrar() {
      this.drawer = this.drawer = !this.drawer;
    },
  },
};
</script>

<style>
</style>
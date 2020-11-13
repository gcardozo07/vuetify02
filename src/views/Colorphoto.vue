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
            <h2>Color in Photography</h2>
          </v-col>
          <v-col class="content-col-1" cols="12" md="6">
            <p>
              Don’t forget that color should be conveyed in large part through
              photography. Here are a few examples of how we’ve edited
              photography to include colors from our palette. All color
              treatment should be natural and authentic.
            </p>
          </v-col>
        </v-row>
        <br /><br />
        <v-row class="row-all">
          <div class="colorphoto">
            <div class="colorphotoin">
              <figure><img src="../img/c1.png" alt="" /></figure>
            </div>
            <div class="colorphotoin">
              <figure><img src="../img/c2.png" alt="" /></figure>
            </div>
            <div class="colorphotoin">
              <figure><img src="../img/c3.png" alt="" /></figure>
            </div>
            <div class="colorphotoin">
              <figure><img src="../img/c4.png" alt="" /></figure>
            </div>
          </div>
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
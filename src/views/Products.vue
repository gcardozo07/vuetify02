<template>
  <v-app>
    <v-navigation-drawer v-model="drawer" absolute temporary>
      <Menu />
    </v-navigation-drawer>
    <v-container class="pa-0">
          <div class="content py-10">
            <Sidebar @accion="mostrar" />
            <v-row>
              <v-col class="content-col-1" cols="12" md="12">
                <h2>All Product Lockups</h2>
              </v-col>
            </v-row>
            <br><br>
            <v-row class="row-all grey lighten-4">
              <v-col class="content-col-1" cols="12" md="6">
                <img src="../img/l1.png" alt="">
              </v-col>
              <v-col class="content-col-1" cols="12" md="6">
                <img src="../img/l2.png" alt="">
              </v-col>
            </v-row>
            <v-row class="row-all">
              <v-col class="content-col-1" cols="12" md="6">
                <img src="../img/l3.png" alt="">
              </v-col>
              <v-col class="content-col-1" cols="12" md="6">
                <img src="../img/l4.png" alt="">
              </v-col>
            </v-row>
            <v-row class="row-all grey lighten-4">
              <v-col class="content-col-1" cols="12" md="6">
                <img src="../img/l5.png" alt="">
              </v-col>
              <v-col class="content-col-1" cols="12" md="6">
                <img src="../img/l6.png" alt="">
              </v-col>
            </v-row>
            <v-row class="row-all">
              <v-col class="content-col-1" cols="12" md="6">
                <img src="../img/l7.png" alt="">
              </v-col>
              <v-col class="content-col-1" cols="12" md="6">
                <img src="../img/l8.png" alt="">
              </v-col>
            </v-row>
            <v-row class="row-all grey lighten-4">
              <v-col class="content-col-1" cols="12" md="6">
                <img src="../img/l9.png" alt="">
              </v-col>
              <v-col class="content-col-1" cols="12" md="6">
                <img src="../img/l10.png" alt="">
              </v-col>
            </v-row>
            <v-row class="row-all">
              <v-col class="content-col-1" cols="12" md="6">
                <img src="../img/l11.png" alt="">
              </v-col>
              <v-col class="content-col-1" cols="12" md="6">
                <img src="../img/l12.png" alt="">
              </v-col>
            </v-row>
          </div>
          <div class="btn-res">
            <a target="_blank" href="https://drive.google.com/drive/folders/1lL8QiZZePkSFCWslfP-vz1gHjMyBEo00?usp=sharing"><img src="../img/arrow.png" alt=""> Go to Resource</a>
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

<style lang="scss">


</style>
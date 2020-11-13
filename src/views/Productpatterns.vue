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
                <h2>Product Patterns</h2>
              </v-col>
            </v-row>
            <br /><br />
            <v-row class="row-all">
              <div class="products-pattern">
              <div class="product"><figure><img src="../img/p1.png" alt="" /></figure></div>
              <div class="product"><figure><img src="../img/p2.png" alt="" /></figure></div>
              <div class="product"><figure><img src="../img/p3.png" alt="" /></figure></div>
              <div class="product"><figure><img src="../img/p4.png" alt="" /></figure></div>
              <div class="product"><figure><img src="../img/p5.png" alt="" /></figure></div>
              <div class="product"><figure><img src="../img/p6.png" alt="" /></figure></div>
          </div>
            </v-row>
          </div>
          <div class="btn-res">
            <a target="_blank" href="https://drive.google.com/drive/folders/120DWf4FbGC30FX8qPdFq95foh4iRZ9cg?usp=sharing"><img src="../img/arrow.png" alt=""> Go to Resource</a>
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
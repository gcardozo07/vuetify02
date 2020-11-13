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
                <h2>Color Assignments</h2>
              </v-col>
              <v-col class="content-col-1" cols="12" md="6">
                <p>You’ll notice that our products utilize specific colors from our palette. Visual design of products
should use their primary colors prominently, supported by their secondary palette.</p>
              </v-col>

            </v-row>
            <br />
            <v-row class="row-all">
              <div class="assignments">
                <div class="assignments-in">
                    <figure>
                       <img src="../img/a1.png" alt="">
                    </figure>
                </div>
                <div class="assignments-in">
                    <figure>
                       <img src="../img/a2.png" alt="">
                    </figure>
                </div>
                <div class="assignments-in">
                    <figure>
                       <img src="../img/a3.png" alt="">
                    </figure>
                </div>
                <div class="assignments-in">
                    <figure>
                       <img src="../img/a4.png" alt="">
                    </figure>
                </div>
                <div class="assignments-in">
                    <figure>
                       <img src="../img/a5.png" alt="">
                    </figure>
                </div>
                <div class="assignments-in">
                    <figure>
                       <img src="../img/a6.png" alt="">
                    </figure>
                </div>
                <div class="assignments-in-2">
                    <figure>
                       <img src="../img/a7.png" alt="">
                    </figure>
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
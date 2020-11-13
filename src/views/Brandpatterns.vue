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
            <h2>Brand Patterns</h2>
            <br><br>
            <p>
              We have developed an entire family of patterns to represent
              various tenets and offerings we provide.
              <br /><br />
              Our extended family of patterns ensures versatility and freshness
              within our design system.
            </p>
            <figure>
              <img class="image-b" src="../img/patt-brand-2.png" alt="" />
            </figure>
          </v-col>
          <v-col
            class="content-col-2 d-flex justify-center align-center"
            cols="12"
            md="6"
          >
            <img class="image-c" src="../img/patt-brand.png" alt="" />
          </v-col>
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
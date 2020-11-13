<template>
  <v-app>
    <v-navigation-drawer v-model="drawer" absolute temporary>
      <Menu />
    </v-navigation-drawer>
    <v-container class="pa-0">
      <v-row>
        <v-col class="pa-0" cols="12" md="12">
          <div class="content py-10">
            <Sidebar @accion="mostrar" />
            <v-row>
              <v-col class="content-col-1" cols="12" md="6">
          <h2>Tagline</h2>
          <br>
          <p>
            We help our customers create better experiences. And our experience
            helps us make sure those experiences matter.
            <br /><br />
            Our tagline helps convey this: Experiences That Matter. The tagline
            should be used whenever space and messaging allow for it.
          </p>
              </v-col>
              <v-col
                class="content-col-2 d-flex justify-center align-center"
                cols="12"
                md="6"
              >
                <img src="../img/avaya-logo-2.png" alt="" />
              </v-col>
            </v-row>
            
            <v-row>
              <v-col class="content-col-1" cols="12" md="6">
          <h2>Logo Crop</h2>
          <br>
          <p>
            Our business is about helping other companies create experiences
            that matter. We always place the customer before ourselves as we are
            a portion—albeit an integral portion—of their experience.
            <br /><br />
            The cropped Avaya logo echoes this notion. We are a part of our
            customers’ stories, helping them create meaningful experiences;
            always supportive, never in the forefront.
          </p>
              </v-col>
              <v-col
                class="content-col-2 d-flex justify-center align-center"
                cols="12"
                md="6"
              >
                <img src="../img/crop.png" alt="" />
              </v-col>
            </v-row>
          </div>
        </v-col>
      </v-row>
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
<template>
<v-app>
  <v-container class="pa-0" fluid>
    <v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
      >
      <Menu />
    </v-navigation-drawer>
    <v-row>

    <v-col class="pa-0" cols="12" md="12">
      <div class="home-in"><Sidebar @accion="mostrar" /></div>
    </v-col>
    </v-row>
  </v-container>
  </v-app>
</template>

<script>
// @ is an alias to /src
import Menu from '../components/Menu'
import Sidebar from '../components/Sidebar'

export default {
  name: 'Home',
    data () {
      return {
        drawer: null,
      }
    },
  components: {
    Menu, Sidebar
  },
  methods:{
    mostrar(){
      this.drawer = this.drawer = !this.drawer
    }
  }
}
</script>
<style lang="scss">
    .home-in{
      width: 100%;
      height: 100vh;
      background-image: url('../img/back.jpg');
      background-size: cover;
      background-position: center;
    }
</style>

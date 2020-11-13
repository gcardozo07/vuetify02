<template>
<div class="fix">
  <v-btn
      color="accent mb-12"
      v-bottom
      @click.stop="accion"
            dark
            absolute
            fab
            elevation="6"
            medium
  
              >
              <v-icon
              
      
      color="white">
      mdi-menu
    </v-icon>
  </v-btn>
</div>

</template>

<script>
export default {
    components:{
        name: 'Sidebar'
    },
    methods: {
      accion(){
        this.$emit('accion')
      }
    }
};
</script>

<style>

.fix {
  position: fixed;
  top: 1.5rem;
  right: 5.5rem;
}
</style>
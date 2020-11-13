<template>
<v-app>
      <div class="menu pa-10">
          <ul>
              <li><router-link to="/">Brand Guidelines</router-link></li>
              <li><span>LOGO & LOGO LOCKUPS</span></li>
              <li><router-link to="/logo">Avaya Logo</router-link></li>
              <li><router-link to="/lockups">Logo Lockups</router-link></li>
              <li><router-link to="/products">Product Lockups</router-link></li>
              <li><span>COLOR</span></li>
              <li><router-link to="/values">Color Values</router-link></li>
              <li><router-link to="/Assignments">Assignments</router-link></li>
              <li><router-link to="/Colorphoto">Color in Photography</router-link></li>
              <li><span>PATTERNS</span></li>
              <li><router-link to="/Brandpatterns">Brand Patterns</router-link></li>
              <li><router-link to="/Productpatterns">Product Patterns</router-link></li>
          </ul>
      </div>
</v-app>
</template>

<script>
export default {
    components:{
        name: 'Menu'
    }
}
</script>

<style lang="scss" scoped>
$color: red;
$noto: "Noto Sans JP";

   .menu {
    height: 100%;
    background: #004E6C;
    box-sizing: border-box;
    background-image: url('../img/patt.png');
    background-size: contain;
    background-repeat: no-repeat;
    background-position: right bottom;
    box-shadow: 2px 4px 10px 8px rgba(0, 0, 0, 0.1);

    ul{
        padding:0;
        li{
            list-style: none;
            padding-bottom: 1rem;
            font-family: $noto;
            text-align: left;
            a{
                color:#fff;
            }
            @media screen and (max-width: 991px) {
                   margin: 0.2rem;
                }
            span{
                color: #45AF9A;
                font-weight: 400;
            }
        }
    }
    h1{
        color: #fff;
    }
}

</style>
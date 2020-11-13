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
                <h2>Color Values</h2>
              </v-col>
            </v-row>
            <br /><br />
            <v-row class="row-all">
              <div class="colors">
          <div class="color-in">
            <div class="color"><span>AVAYA RED</span></div>
            <div class="color-data">
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>HEX</b><br />
                    DA291C</span
                  >
                </div>
                <div>
                  <span
                    ><b>CMYK</b><br />
                    9 97 100 1</span
                  >
                </div>
              </div>
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>RGB</b><br />
                    218 41 28</span
                  >
                </div>
                <div>
                  <span
                    ><b>PANTONE</b><br />
                    485 C</span
                  >
                </div>
              </div>
            </div>
          </div>

          <div class="color-in">
            <div class="color"><span>SUNSET</span></div>
            <div class="color-data">
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>HEX</b><br />
                    EA6834</span
                  >
                </div>
                <div>
                  <span
                    ><b>CMYK</b><br />
                    3 73 91 0</span
                  >
                </div>
              </div>
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>RGB</b><br />
                    234 104 52</span
                  >
                </div>
                <div>
                  <span
                    ><b>PANTONE</b><br />
                    7578 C</span
                  >
                </div>
              </div>
            </div>
          </div>

          <div class="color-in">
            <div class="color"><span>MERIGOLD</span></div>
            <div class="color-data">
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>HEX</b><br />
                    EA8C3F</span
                  >
                </div>
                <div>
                  <span
                    ><b>CMYK</b><br />
                    5 53 85 0</span
                  >
                </div>
              </div>
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>RGB</b><br />
                    234 140 63</span
                  >
                </div>
                <div>
                  <span
                    ><b>PANTONE</b><br />
                    7413 C</span
                  >
                </div>
              </div>
            </div>
          </div>

          <div class="color-in">
            <div class="color"><span>TEAL</span></div>
            <div class="color-data">
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>HEX</b><br />
                    0A8E9B</span
                  >
                </div>
                <div>
                  <span
                    ><b>CMYK</b><br />
                    83 27 36 2</span
                  >
                </div>
              </div>
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>RGB</b><br />
                    10 142 155</span
                  >
                </div>
                <div>
                  <span
                    ><b>PANTONE</b><br />
                    2461 C</span
                  >
                </div>
              </div>
            </div>
          </div>

          <div class="color-in">
            <div class="color"><span>JADE</span></div>
            <div class="color-data">
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>HEX</b><br />
                    45AF9A</span
                  >
                </div>
                <div>
                  <span
                    ><b>CMYK</b><br />
                    70 8 48 0</span
                  >
                </div>
              </div>
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>RGB</b><br />
                    69 175 154</span
                  >
                </div>
                <div>
                  <span
                    ><b>PANTONE</b><br />
                    7723 C</span
                  >
                </div>
              </div>
            </div>
          </div>

          <div class="color-in">
            <div class="color"><span>DENIM</span></div>
            <div class="color-data">
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>HEX</b><br />
                    004E6C</span
                  >
                </div>
                <div>
                  <span
                    ><b>CMYK</b><br />
                    97 66 38 21</span
                  >
                </div>
              </div>
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>RGB</b><br />
                    0 78 108</span
                  >
                </div>
                <div>
                  <span
                    ><b>PANTONE</b><br />
                    2153 C</span
                  >
                </div>
              </div>
            </div>
          </div>

          <div class="color-in">
            <div class="color"><span>OCEAN</span></div>
            <div class="color-data">
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>HEX</b><br />
                    1B77AF</span
                  >
                </div>
                <div>
                  <span
                    ><b>CMYK</b><br />
                    86 48 10 0</span
                  >
                </div>
              </div>
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>RGB</b><br />
                    27 119 175</span
                  >
                </div>
                <div>
                  <span
                    ><b>PANTONE</b><br />
                    2383 C</span
                  >
                </div>
              </div>
            </div>
          </div>

          <div class="color-in">
            <div class="color"><span>BLACK</span></div>
            <div class="color-data">
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>HEX</b><br />
                    000000</span
                  >
                </div>
                <div>
                  <span
                    ><b>CMYK</b><br />
                    0 0 0 100</span
                  >
                </div>
              </div>
              <div class="data-col">
                <div style="padding-bottom: 6px">
                  <span
                    ><b>RGB</b><br />
                    0 0 0
                  </span>
                </div>
                <div>
                  <span
                    ><b>PANTONE</b><br />
                    Black 6 C</span
                  >
                </div>
              </div>
            </div>
          </div>

          <div class="color-in-2">
            <div class="blt">
              <div style="background:#333333" class="color"></div>
              <div class="color-data">
                <div class="data-col">
                  <div style="padding-bottom: 6px">
                    <span
                      ><b>HEX</b><br />
                      333333</span
                    >
                  </div>
                  <div style="padding-bottom: 6px">
                    <span
                      ><b>CMYK</b><br />
                      0 0 0 94</span
                    >
                  </div>
                </div>
                <div class="data-col">
                  <div style="padding-bottom: 6px">
                    <span
                      ><b>RGB</b><br />
                      51 51 51
                    </span>
                  </div>
                </div>
              </div>
            </div>
            <div class="blt">
              <div style="background:#F5F5F5" class="color"></div>
              <div class="color-data">
                <div class="data-col">
                  <div style="padding-bottom: 6px">
                    <span
                      ><b>HEX</b><br />
                      F5F5F5</span
                    >
                  </div>
                  <div style="padding-bottom: 6px">
                    <span
                      ><b>CMYK</b><br />
                      0 0 0 4</span
                    >
                  </div>
                </div>
                <div class="data-col">
                  <div style="padding-bottom: 6px">
                    <span
                      ><b>RGB</b><br />
                      245 245 245 
                    </span>
                  </div>
                </div>
              </div>
            </div>
            <div class="blt">
              <div style="background:#E6E6E6" class="color"></div>
              <div class="color-data">
                <div class="data-col">
                  <div style="padding-bottom: 6px">
                    <span
                      ><b>HEX</b><br />
                      E6E6E6</span
                    >
                  </div>
                  <div style="padding-bottom: 6px">
                    <span
                      ><b>CMYK</b><br />
                      0 0 0 11</span
                    >
                  </div>
                </div>
                <div class="data-col">
                  <div style="padding-bottom: 6px">
                    <span
                      ><b>RGB</b><br />
                      230 230 230 
                    </span>
                  </div>
                </div>
              </div>
            </div>
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
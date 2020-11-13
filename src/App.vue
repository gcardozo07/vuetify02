<template>
  <v-app>
    <router-view />
  </v-app>
</template>

<script>
export default {
  name: "App",

  components: {},

  data: () => ({
    //
  }),
};
</script>



<script>
import Menu from "./components/Menu";
export default {
  components: {
    Menu,
  },
};
</script>


<style lang="scss">
$noto: "Noto Sans JP";

.content-col-1 {
  .image-b {
    width: 380px;
  }
  h2 {
    font-family: $noto;
    border-left: 8px solid #da291c;
    padding-left: 1rem;
    font-size: 2.5rem;
    color: #000;
  }
  p {
    font-family: $noto;
    font-size: 0.9rem;
    line-height: 1.5rem;
  }
  img {
    width: 100%;
    padding-top: 0.5rem;
  }
}

.content-col-2 {
  padding: 1rem 2rem;
  img {
    width: 350px;
    padding-top: 2rem;
  }
  .image-c {
    width: 90%;
  }
}

.row-all {
  display: flex;
  @media screen and (max-width: 991px) {
    flex-direction: column;
  }
  figure {
    margin: 0;
    img {
      padding-top: 2rem;
      width: 100%;
    }
  }
}


a {
  font-weight: 400;
  color: #ffffff;
  text-decoration: none;
  transition: all 0.3s ease 0s;
}

a.router-link-exact-active {
  color: #fff;
  font-weight: 700;
  text-decoration: none;
  border: 1px solid #fff;
  transition: all 0.3s ease 0s;
  padding: 0.2rem 0.2rem;
}

.sidebar {
  @media screen and (max-width: 991px) {
    width: 100%;
  }
}
.content {
  padding: 3rem;
  text-align: left;

  .row-all {
    display: flex;
    @media screen and (max-width: 991px) {
      flex-direction: column;
    }
    figure {
      margin: 0;
      img {
        padding-top: 2rem;
        width: 100%;
      }
    }

    h1 {
      font-size: 3rem;
      color: #000;
      font-family: $noto;
      font-weight: 700;
      border-left: 8px solid #da291c;
      padding-left: 1rem;
      text-align: left;
      margin: 0;
    }
    h2 {
      font-family: $noto;
      border-left: 8px solid #da291c;
      padding-left: 1rem;
      font-size: 2rem;
      color: #000;
    }
    p {
      font-family: $noto;
      font-size: 0.9rem;
      line-height: 1.5rem;
    }
    .assignments {
      display: flex;
      width: 100%;
      justify-content: space-evenly;
      flex-wrap: wrap;
      .assignments-in {
        width: 200px;
        min-height: 200px;
        margin: 1rem;
        figure {
          img {
            width: 100%;
          }
        }
      }
      .assignments-in-2 {
        width: 430px;
        min-height: 180px;
        border: 1px solid #ccc;
        figure {
          display: flex;
          align-items: center;
          justify-content: center;
          img {
            width: 55%;
          }
        }
      }
    }
    .colorphoto {
      width: 100%;
      display: flex;
      justify-content: space-evenly;
      flex-wrap: wrap;
      .colorphotoin {
        width: 220px;
        margin: 0.2rem;
        figure {
          img {
            width: 100%;
          }
        }
      }
    }
    .products-pattern {
      width: 100%;
      display: flex;
      justify-content: space-evenly;
      flex-wrap: wrap;
      .product {
        width: 320px;
        figure {
          img {
            width: 100%;
          }
        }
      }
    }
  }

  .colors {
    width: 100%;
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;

    .color-in {
      width: 160px;
      background: #da291c;
      text-align: center;
      box-shadow: 2px 4px 10px 8px rgba(0, 0, 0, 0.1);
      margin: 0.8rem 0.5rem;
      transition: all 0.4s ease 0s;
      flex: 1 1 auto;
      &:hover {
        box-shadow: 2px 5px 12px 0 rgba(0, 0, 0, 0.3);
        transition: all 0.4s ease 0s;
      }
      &:nth-child(2) {
        background: #ea6834;
      }
      &:nth-child(3) {
        background: #ea8c3f;
      }
      &:nth-child(4) {
        background: #0a8e9b;
      }
      &:nth-child(5) {
        background: #45af9a;
      }
      &:nth-child(6) {
        background: #004e6c;
      }
      &:nth-child(7) {
        background: #1b77af;
      }
      &:nth-child(8) {
        background: #000000;
      }
      .color {
        width: 100%;
        min-height: 150px;
        padding: 1rem;
        box-sizing: border-box;
        span {
          color: #fff;
          text-align: center;
          font-family: $noto;
          font-size: 0.8rem;
        }
      }
      .color-data {
        background: #fff;
        padding: 1rem;
        display: flex;
        justify-content: space-between;
        .data-col {
          text-align: left;
          font-family: $noto;
          font-size: 0.8rem;
          span {
            color: #333;
          }
        }
      }
    }
    .color-in-2 {
      width: 380px;
      background: #fff;
      box-shadow: 2px 4px 10px 8px rgba(0, 0, 0, 0.2);
      margin: 0.8rem 0.5rem;
      display: flex;
      transition: all 0.4s ease 0s;
      flex: 1 1 auto;
      &:hover {
        box-shadow: 2px 5px 12px 0 rgba(0, 0, 0, 0.3);
        transition: all 0.4s ease 0s;
      }
      .blt {
        width: 33.33%;
        .color-data {
          background: #fff;
          padding: 0.8rem;
          justify-content: space-between;
          .data-col {
            text-align: left;
            font-family: $noto;
            font-size: 0.7rem;
            span {
              color: #333;
              text-align: center;
            }
          }
        }
        .color {
          width: 100%;
          min-height: 120px;
          padding: 1rem;
          box-sizing: border-box;
          span {
            color: #fff;
            text-align: center;
            font-family: $noto;
            font-size: 0.8rem;
          }
        }
      }
    }
  }
}
.btn-res {
  width: 175px;
  min-height: 40px;
  border-radius: 1.2rem;
  background: #da291c;
  position: absolute;
  bottom: 2rem;
  right: 2rem;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.5s ease 0s;
  color: #fff;
  &:hover {
    background: #c00;
    box-shadow: 2px 4px 10px 3px rgba(0, 0, 0, 0.2);
    img {
      padding-left: 4px;
    }
  }
  a {
    font-family: $noto;
    font-weight: 700;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #ffffff !important;

    img {
      width: 25px;
      padding-right: 5px;
      transition: all 0.2s ease 0s;
    }
  }
}
</style>

<template>
  <div id="main">
    <div id="navbar">
      <vs-navbar
        fixed="true"
        center-collapsed
        v-model="active"
        id="header"
        text-white
        color="#072b43">
        <vs-navbar-item  v-on:click="scrollToHome()" id="guide">
          Accueil
        </vs-navbar-item>
        <vs-navbar-item  v-on:click="scrollToPresentation()" id="docs">
          Présentation
        </vs-navbar-item>
        <vs-navbar-item  v-on:click="scrollToProjet()" id="components">
          Projet Professionnel
        </vs-navbar-item>
        <vs-navbar-item  v-on:click="scrollToPortfolio()" id="license">
          Portfolio
        </vs-navbar-item>
      </vs-navbar>
    </div>

    <MainPage v-on:presentation="scrollToPresentation()" v-on:projet="scrollToProjet()" v-on:portfolio="scrollToPortfolio()" ></MainPage>

    <hr class="hr">

    <Presentation id="presentation" class="composant"></Presentation>
    <div id="CV" class="composant">
      <div id="buttonDiv">
        <vs-button
          id="CVButton"
          color="#316a84"
          border
        >
          <a href="/CV_Lucas_Pastori.pdf" download="">CV</a>
        </vs-button>
      </div>
    </div>


    <hr class="hr">
    <ProjetPro id="projet" class="composant"></ProjetPro>
    <hr class="hr">
    <Portfolio id="portfolio" class="composant"></Portfolio>
  </div>
</template>

<script>

import MainPage from '~/components/MainPage.vue'
import Header from "../components/Header";
import Presentation from "../components/Presentation";
import ProjetPro from "../components/ProjetPro";
import Portfolio from "../components/Portfolio";

export default {
  components: {
    Portfolio,
    ProjetPro,
    MainPage,
    Header,
    Presentation,
  },
  data(){
    return {
      publicPath: process.env.BASE_URL
    }
  },
  methods: {
    scrollToHome(){
      window.scrollTo({top: 0, behavior: 'smooth'});
    },
    scrollToPresentation(){
      let container = document.getElementById("presentation");
      container.scrollIntoView({behavior: "smooth"});
    },
    scrollToProjet(){
      let container = document.getElementById("projet");
      container.scrollIntoView({behavior: "smooth"});
    },
    scrollToPortfolio(){
      let container = document.getElementById("portfolio");
      container.scrollIntoView({behavior: "smooth"});
    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 55px;
  color: #35495e;
  letter-spacing: 1px;
  text-transform: capitalize;
  margin: 25px 0;
}

.subtitle {
  font-weight: 300;
  font-size: 1.1rem;
  color: #526488;
  word-spacing: 2px;
  padding-bottom: 15px;
  max-width: 600px;
}

.subtitle a {
  font-weight: 500;
  color: inherit;
}

.links {
  padding-top: 15px;
  margin-bottom: 20px;
}

.content-logos {
  display: flex;
  align-items: center;
  justify-content: center;
  min-width: 500px;
}

.plus {
  font-size: 2.5rem;
  margin: 15px;
  color: #35495e;
}

.h3 {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-weight: 400;
  margin: 10px;
}

#buttonDiv{
  margin-top: 5%;
  height: 20%;
}
#CVButton{
  float: none;
  margin-left: auto;
  margin-right: auto;
  width: 10%;
  height: 5%;
  color: #316a84;
}

.hr{
  border: 2px solid #35495e;
  margin:2% 7% 0% 7%;
}

#header{
  height: 5%;
  font-family: Roboto, sans-serif;
}

  #main{
    margin-bottom: 5%;
  }
  .composant{
    padding-top: 3%;
  }
</style>

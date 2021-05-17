<template>
  <div id="main">
    <h1 id="title"> BIENVENUE SUR LE SITE PORTFOLIO DE LUCAS PASTORI</h1>
    <hr class="hr">
    <div id="rectangles">
        <div id="rect1" >
          <vs-button
            id ='buttonPresentation'
            border
            color="#f7f8fb"
            padding-top="85px"
            :active="active === 1"
            v-on:click="$emit('presentation')"
          >Présentation</vs-button>
        </div>
        <div id="rect2" v-on:click="$emit('projet')">
          <vs-button
            id ='buttonProjet'
            border
            color="#f7f8fb"
            padding-top="85px"
            :active="active === 1"
            @click="active = 1"
          >Projet professionnel</vs-button>
        </div>
        <div id="rect3" v-on:click="$emit('portfolio')">
          <vs-button
            id ='buttonPortfolio'
            border
            color="#f7f8fb"
            padding-top="85px"
            :active="active === 1"
            @click="active = 1"
          >Portfolio</vs-button>
        </div>
    </div>
    <hr class="hr">
    <div id="next">
      <img src="./../assets/fleche.png" alt="fleche next" id="flecheNext"  v-on:click="$emit('presentation')">
    </div>
  </div>
</template>

<script>
    export default {
        name: "MainPage"
    }
</script>

<style scoped>
  #main{
    background-image: url("./../assets/fondflou.jpg");
    background-size: 100%;
    width: 100%;
    height:100%;
  }
  #title{
    font-family: Roboto,sans-serif;
    font-weight: lighter;
    color: #ffffff;
    text-align: center;
    padding-top: 6% ;
    font-size: 40px;
    letter-spacing: 8px;
  }
  #rectangles{
    padding: 7%;
    display: flex;
  }
  .hr{
    border: 1px solid white;
    margin:2% 7% ;
    display: block;
  }
  #rect1{
    flex: 1;
    margin-right: 7%;
  }
  #rect2{
    flex: 1;
    margin-right: 7%;
  }
  #rect3{
    flex: 1;

  }
  #buttonProjet{
    margin-left: auto;
    margin-right: auto;
    height: 125px;
    width: 250px;
    font-size: 25px;
    font-family: Roboto, sans-serif;
    color: #f7f8fb;
    transition-delay: 10ms;
    background-color: #e08e7a;
    box-shadow: 2px 0px 3px black;
  }
  #buttonProjet:hover{
    flex: 1;
    box-shadow: 2px 0px 10px black;
    margin-left: auto;
    margin-right: auto;
    color: rgba(0, 0, 0, 0);
    transform: scale(2.0); /*Add this*/
    background-image :url("./../assets/projet_screen.png");
    background-size: 250px 120px;
  }
  #buttonPortfolio{
    margin-left: auto;
    margin-right: auto;
    height: 125px;
    width: 250px;
    font-size: 25px;
    font-family: Roboto, sans-serif;
    background-color: #316a84;
    color: #f7f8fb;
    transition-delay: 10ms;
    box-shadow: 2px 0px 3px black;
  }
  #buttonPortfolio:hover{
    margin-left: auto;
    margin-right: auto;
    background-color: #316a84;
    box-shadow: 2px 0px 10px black;
    color: rgba(0, 0, 0, 0);
    transform: scale(2.0); /*Add this*/
    background-image :url("./../assets/portfolio_scrren.png");
    background-size: 250px 120px;
  }
  #buttonPresentation{
    margin-left: auto;
    margin-right: auto;
    flex: 1;
    height: 125px;
    width: 250px;
    font-size: 25px;
    font-family: Roboto, sans-serif;
    background-color: #072b43;
    color: #f7f8fb;
    transition-delay: 10ms;
    box-shadow: 2px 0px 3px black;
  }
  #buttonPresentation:hover{
    margin-left: auto;
    margin-right: auto;
    flex: 1;
    background-color: #072b43;
    box-shadow: 2px 0px 10px black;
    transform: scale(2.0); /*Add this*/
    color: rgba(0, 0, 0, 0);
    background-image :url("./../assets/presentation_screen.png");
    background-size: 250px 120px;
  }
  #flecheNext{
    height: 70px;
    padding-top: 20px;
    margin-bottom: 8%;
    margin-left: auto;
    margin-right: auto;
    width: 50px;
  }
  #next{
    display: flex;
  }
  #next:hover{

  }

</style>

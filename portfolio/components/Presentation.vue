<template>
  <div>
    <div>
      <div id="title">
        <a>PRESENTATION</a>
      </div>
      <div id="text-flex">
        <img src="./../assets/Lulu.jpg" alt="photo de Lucas" id="Photo">
        <div id="sous-text">
          <span class="bold">Lucas Pastori</span><br>
          Etudiant en informatique,<br>
          EPHEC Louvain-la-Neuve
        </div>
        <div id="text">
          Habitant actuellement à Andenne, je suis un jeune étudiant dynamique de 20 ans en 3ème année de son bachelier informatique à l'EPHEC de Louvain-La-Neuve.<br><br>

          J'ai choisi l'informatique car c'est un thème m'ayant toujours intéressé et étant un fan de jeux vidéo en tous genres, je voulais pouvoir m'imaginer comment ceux-ci sont créés.<br><br>

          <b>Compétences :</b><br>
          <br>
          Grâce à l'EPHEC et à mes études secondaires, j'ai pu acquérir diverses compétences.<br><br>
          En premier lieu, j'ai appris la suite Adobe dans mes différents cours d'infographie.<br><br>
          Ensuite, dans le cadre de mes études à l'EPHEC, j'ai pu découvrir plusieurs aspects de l'informatique tels que la programmation, l'électronique digitale, l'infrastructure réseau, ...<br>
          Parmi ces différents cours, j'ai passé le plus de temps à me former à la programmation en essayant de maîtriser le Javascript qui est le langage avec lequel je me sens le plus à l'aise. Je possède de solides bases en électronique et en réseau car ce sont des sujets qui m'intéressent aussi.<br><br>
          Je tiens aussi à préciser que je possède un bon niveau en anglais.

        </div>
      </div>

    </div>

  </div>
</template>

<script>
    export default {
        name: "Presentation"
    }
</script>

<style scoped>
#Photo{
  height:10%;
  width: 10%;
  border-radius: 50%;
  box-shadow: 2px 0px 6px black;
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 1%;
}

#title{
  text-align: center;
  font-family: Roboto,sans-serif;
  margin-bottom: 3%;
  font-weight: lighter;
  font-size: 250%;
  letter-spacing: 12px;
}
.hr{
  border: 1px dashed #e08e7a;
  margin: -1% 39% 3%;
}
#text-flex{

}
#text{
  width: 60%;
  text-align: justify;
  margin-left: auto;
  margin-right: auto;
  font-size: 110%;
}
#sous-text{
  text-align: center;
  font-family: Roboto,sans-serif;
  font-size: 120%;
  margin-bottom: 3% ;
}
.bold{
  font-weight: bold;
}

</style>

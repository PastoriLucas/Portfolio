<template>
  <div id="main">
    <div id="title">
      <a> PORTFOLIO </a>
    </div>
    <div>
      <div >
        <div id="tableDiv">
          <table id="table">
              <tr id="tr">
                <th class="th">
                </th>
                <th class="th">
                  Nom
                </th>
                <th class="th">
                  Type
                </th>
                <th class="th">
                  Heures totale
                </th>
                <th class="th">
                  Heures prestées
                </th>
              </tr>

              <tr @click="actif1=true" class="row">
                <td>
                  1
                </td>
                <td>
                  Cyber security challenge
                </td>
                <td>
                  Capture the flag
                </td>
                <td>
                  96
                </td>
                <td>
                  10
                </td>
              </tr>
              <tr @click="actif2=true" class="row">
                <td>
                  2
                </td>
                <td>
                  Travail chez "Lhoist"
                </td>
                <td>
                  Job étudiant
                </td>
                <td>
                  210
                </td>
                <td>
                  10
                </td>
              </tr>
              <tr @click="actif3=true" class="row">
                <td>
                  3
                </td>
                <td>
                  Aprentissage Illustrator
                </td>
                <td>
                  Formation en ligne
                </td>
                <td>
                  12
                </td>
                <td>
                  10
                </td>
              </tr>
              <tr @click="actif4=true" class="row">
                <td>
                  4
                </td>
                <td>
                  Aprentissage NodeJs
                </td>
                <td>
                  Formation en ligne
                </td>
                <td>
                  10
                </td>
                <td>
                  10
                </td>
              </tr>
              <tr @click="actif5=true" class="row">
                <td>
                  5
                </td>
                <td>
                  Aprentissage PHP / Mysql
                </td>
                <td>
                  Formation en ligne
                </td>
                <td>
                  70
                </td>
                <td>
                  10
                </td>
              </tr>
              <tr @click="actif6=true" class="row">
                <td>
                  6
                </td>
                <td>
                  UTCTF
                </td>
                <td>
                  Capture the flag
                </td>
                <td>
                  14
                </td>
                <td>
                  10
                </td>
              </tr>
              <tr @click="actif7=true" class="row">
                <td>
                  7
                </td>
                <td>
                  Formation Gimp
                </td>
                <td>
                  Formation en ligne
                </td>
                <td>
                  2
                </td>
                <td>
                  0
                </td>
              </tr>
              <tr @click="actif8=true" class="row">
                <td>
                  8
                </td>
                <td>
                  RootMe
                </td>
                <td>
                  Capture the flag
                </td>
                <td>
                  14
                </td>
                <td>
                  0
                </td>
              </tr>

              <tr >
                <td class="bold">
                  TOTAL
                </td>
                <td>

                </td>
                <td>

                </td>
                <td class="total">
                  428
                </td>
                <td class="total">
                  60
                </td>
              </tr>
          </table>
        </div>
        <vs-dialog overflow-hidden full-screen v-model="actif1">
        <template #header>
          <h4 class="dialog-title">
            <b>Cyber security challenge</b>
          </h4>
        </template>
          <img src="../assets/CSCB.png" alt="Cyber security challenge logo" class="logo">
        <div class="con-content">
          <p>
            Lors de mes 3 années à l'EPHEC, j'ai participé plusieurs fois au <span class="bold">Cyber Security Challenge Belgium</span>.<br>
            Le Cyber Security Challenge est une compétition de capture the flag accessible uniquement aux étudiants qui se déroule au mois de mars de chaque année.<br>
            La compétition est divisée en plusieurs parties commençant par les qualifications qui durent 32 heures à chaque édition. Je n'expliquerai pas plus loin que les qualifications car je n'ai jamais passé celles-ci.<br>
            Pour ce qui est du but, le principe d'un "capture the flag" est de retrouver des flags (drapeaux) cachés à différents endroits dans différentes énigmes toutes plus ou moins faciles.<br>
            Toutes ces énigmes demandent la plupart du temps des connaissances en informatiques et sont souvent regroupées en domaines tels que le "reverse engineering", la stéganographie, etc.<br>
            <br>
            J'y ai participé lors de ma première année en n'attendant pas grand-chose au niveau des résultats de mon équipe (uniquement constituée de 1ère année) et au niveau de la compétition en elle-même (je pensais vite en être lassé et arrêter).<br>
            Pour finir , j'ai vraiment pris goût au format et me suis fortement amusé à participer chaque année à cette compétition avec mon groupe d'amis.<br>
            <br>
            De plus, cette compétition m'a appris beaucoup de choses.<br>
            Elle m'a permis de découvrir la stéganographie que je trouve particulièrement intéressante. Celle-ci je pense m'avait déjà légèrement préparé au cours de "Traitement des signaux" de par son approche à sortir une certaine donnée d'une image ou d'un son.<br>
            Elle nous a aussi permis de mieux comprendre la programmation grâce à ces différentes épreuves en nous demandant de créer de petits programmes nous permettant d'atteindre notre but.<br>
            Je tiens aussi à dire que la plupart des épreuves demandent de savoir utiliser Linux et les commandes de base du système ce qui m'a permis d'avoir certains déclics.<br>
            <br>
            Pour conclure, j'aimerais le conseiller à tous les étudiants ayant l'occasion d'y participer (qu'ils soient dans le milieu de l'informatique ou non).<br>
            C'est vraiment une expérience enrichissante à laquelle on prend goût si on lui laisse une chance et qui nous a permis de resserrer les liens entre les membres de mon groupe.

          </p>
          <div class="flex">
            <vs-button class="preuve" @click="preuveCSC1=true">preuve 1</vs-button>
            <vs-button class="preuve" @click="preuveCSC2=true">preuve 2</vs-button>
            <vs-button class="preuve" @click="preuveCSC3=true">preuve 3</vs-button>
          </div>

        </div>

      </vs-dialog>
        <vs-dialog overflow-hidden full-screen v-model="actif2">
          <template #header>
            <h4 class="dialog-title">
              <b>Lhoist</b>
            </h4>
          </template>
          <img src="../assets/LHOIST.jpg" alt="Lhoist logo" class="logo">
          <div class="con-content">
            <p>
              J'ai eu la chance de travailler chaque année pendant 2 semaines chez Lhoist en tant qu'étudiant.<br>
              Lhoist est une entreprise spécialisée dans la production de chaux et de chaux dolomiques ainsi que dans l'extraction de minéraux.<br>
              <br>
              Lors de ce stage, j'ai reçu différentes tâches allant de l'administratif (gestion de documents) à la remise en couleurs de plusieurs locaux tout en étant au services des différentes branches de la boîte.<br>
              <br>
              Malgré le fait que mes tâches n'aient pas de rapport direct à l'informatique,
              ce job étudiant m'a permis d'avoir ma première expérience professionnelle et de me préparer pour les autres à venir.<br>
              Celui-ci m'a aussi mieux fait comprendre comment marche une société ce qui peut s'avérer fortement utile dans le cadre professionnel en général.
            </p>
          </div>
          <div class="flex">
            <vs-button class="preuve" @click="preuveLhoist=true">preuve</vs-button>
          </div>
        </vs-dialog>
        <vs-dialog overflow-hidden  full-screen v-model="actif3">
          <template #header>
            <h4 class="dialog-title">
              <b>Formation Illustrator</b>
            </h4>
          </template>
          <img src="../assets/illustrator.png" alt="Illustrator logo" class="logo">
          <div class="con-content">
            <p>
              J'ai eu l'occasion de réaliser la formation "Créez des visuels avec Illustrator" venant d'OpenClassrooms.<br>
              <br>
              Etant fortement intéressé par le design, cette formation me semblait être un plus pour le métier de développeur Web.<br>
              Malgré le fait que la formation ne dure que 10 heures, celle-ci repasse sur certains principes de design intéressant pouvant être utiles à la plupart des programmeurs frontend.<br>
              De plus, couplé avec mes connaissances en Photoshop, cette formation me permet de créer des maquettes complètes de sites avant de les réaliser afin de ne pas perdre de temps avec la mise en place des différents composants des sites web sur lesquels je travaille.<br>
              <br>
              Cette formation m'a rappelé des techniques de design intéressantes qui a mes yeux sont un gros plus pour les développeurs voulant se démarquer de la masse grâce a leur polyvalence.
            </p>
          </div>

          <div class="flex">
            <vs-button class="preuve" @click="preuveIlu1=true">preuve 1</vs-button>
            <vs-button class="preuve" @click="preuveIlu2=true">preuve 2</vs-button>
            <vs-button class="preuve" @click="preuveIlu3=true">preuve 3</vs-button>
          </div>
        </vs-dialog>
        <vs-dialog overflow-hidden full-screen v-model="actif4">
          <template #header>
            <h4 class="dialog-title">
              <b>Formation NodeJs</b>
            </h4>
          </template>
          <img src="../assets/NodeJs.png" alt="NodeJs logo" class="logo">
          <div class="con-content">
            <p>
              J'ai eu l'occasion de réaliser la formation "Des applications ultra rapides avec NodeJs" venant d'OpenClassrooms.<br>
              <br>
              Cette formation m'a fortement été utile dans le cadre du projet d'intégration que nous réalisons en 3ème année et dans le cadre de la création d'un site web pour notre projet de 2ème année.<br>
              Etant principalement attiré par le langage de programmation javascript, apprendre NodeJs me semblait nécessaire dans mon développement afin de pouvoir travailler en web.<br>
              Cette formation m'a beaucoup appris. Elle m'a fait découvrir et mieux comprendre comment marche le backend d'une application. Créer mes premières APIs rest.
              Et fait réaliser l'existence des nombreux packages npm pouvant s'avérer extrêmement utile en nous évitant de réinventer la roue.
            </p>
          </div>
          <div class="flex">
            <vs-button class="preuve" @click="preuveNode1=true">preuve 1</vs-button>
            <vs-button class="preuve" @click="preuveNode2=true">preuve 2</vs-button>
            <vs-button class="preuve" @click="preuveNode3=true">preuve 3</vs-button>
          </div>

        </vs-dialog>
        <vs-dialog overflow-hidden full-screen v-model="actif5">
          <template #header>
            <h4 class="dialog-title">
              <b>Formation PHP / MySql</b>
            </h4>
          </template>
          <img src="../assets/PHP_mySql.png" alt="PHP logo" class="logo">
          <div class="con-content">
            <p>
              J'ai eu l'occasion de réaliser la formation "Concevez votre site web avec PHP et MySQL" venant d'OpenClassrooms.<br>
              <br>
              Cette formation m'a fait découvrir les bases du PHP que je n'ai pas eu l'occasion de voir en cours.
              j'ai commencé cette formation afin d'être prêt a toute éventualité dans le cadre de mon stage et pour finir je n'ai pas eu à programmer en PHP, mais celle-ci reste très intéressante.<br>
              Elle revient sur certains points nécessaires à la programmation (boucles, conditions, ...) dans le cadre du PHP et se permet même de nous apprendre des choses plus utiles tel que les bases du Regex.<br>
              La formation nous apprend aussi à utiliser MySQL tout en expliquant brièvement les concepts de base des bases de données.<br>
              <br>
              Cette formation m'a été utile car elle m'a fait découvrir un nouveau langage. Elle m'a également fait revoir les principes fondamentaux de la programmation avant mon stage ce qui m'a permis de me sentir un peu plus à l'aise.
            </p>
          </div>
          <div class="flex">
            <vs-button class="preuve" @click="preuvePHP1=true">preuve 1</vs-button>
            <vs-button class="preuve" @click="preuvePHP2=true">preuve 2</vs-button>
            <vs-button class="preuve" @click="preuvePHP3=true">preuve 3</vs-button>
          </div>

        </vs-dialog>
        <vs-dialog overflow-hidden full-screen v-model="actif6" >
          <template #header>
            <h4 class="dialog-title">
              <b>UTCTF 2021</b>
            </h4>
          </template>
          <img src="../assets/utctf.jpg" alt="UTCTF logo" class="logo">
          <div class="con-content">
            <p>
              UTCTF est une compétition de "capture the flag" connue se déroulant chaque année (comme le CSCB).<br>
              Le principe d'un "capture the flag" est de retrouver des flags (drapeaux) cachés à différents endroits dans différentes énigmes toutes plus ou moins faciles.<br>
              Toutes ces énigmes demandent la plupart du temps des connaissances en informatiques et sont souvent regroupés en domaines tels que le "reverse engineering", la stéganographie, etc.<br>
              <br>
              Comme dit précédemment dans l'onglet traitant du CSCB les compétitions de "Capture the flag" nous font découvrir plein de technologies et d'aspects de la sécurité auxquels on ne pense pas toujours.<br>
              Cette compétition en particulier m'a beaucoup fait pratiquer le "reverse engineering" dont le principe est d'analyser un code afin de trouver comment le modifier pour trouver un flag.
            </p>
          </div>
          <div class="flex">
            <vs-button class="preuve" @click="preuveUTCTF1=true">preuve 1</vs-button>
            <vs-button class="preuve" @click="preuveUTCTF2=true">preuve 2</vs-button>
          </div>
        </vs-dialog>

        <vs-dialog overflow-hidden full-screen v-model="actif7">
          <template #header>
            <h4 class="dialog-title">
              <b>Formation GIMP</b>
            </h4>
          </template>
          <img src="../assets/GIMP.png" alt="GIMP logo" class="logo">
          <div class="con-content">
            <p>
              Lors d'un évènement Louvain-li-nux, j'ai pu m'intéresser à une formation en live de GIMP.<br>
              Cette formation couplée avec mes connaissances en Photoshop me permet de réaliser des maquettes pour mes différentes applications sans devoir payer la License Adobe.<br>
              Celle-ci repassait sur les grands points du logiciel et sur ce que l'on peut faire avec celui-ci.
            </p>
          </div>
          <div class="flex">
            <vs-button class="preuve" @click="preuveGIMP=true">preuve</vs-button>
          </div>
        </vs-dialog>

          <vs-dialog overflow-hidden full-screen v-model="actif8">
            <template #header>
              <h4 class="dialog-title">
                <b>RootMe</b>
              </h4>
            </template>
            <img src="../assets/rootme.png" alt="rootMe logo" class="logo">
            <div class="con-content">
              <p>
                Lors de mon temps libre, j'ai aussi participer a du "capture the flag" sur le site RootMe.<br>
                Le site propose des épreuves allant de simple à très dur avec une belle courbe de progression, et traite de tout les thèmes que l'on peut rencontrer dans les vraies compétitions.<br>
                De plus, pour la plupart des épreuves, le site donne à ses utilisateurs des documentations complètes pouvant donner une piste sur comment résoudre les énigmes.<br>
                Enfin un dernier bon point est qu'une fois qu'une épreuve est réussie, les utilisateurs ont accès à toutes les solutions possibles connues par la communauté.
              </p>
            </div>
          </vs-dialog>


        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuveCSC1" >
          <img alt="preuve csc 1" src="../assets/CSCB_preuve_1.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuveCSC2" >
          <img alt="preuve csc 1" src="../assets/CSCB_preuve_2.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuveCSC3" >
          <img alt="preuve csc 1" src="../assets/CSCB_preuve_3.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuveLhoist" >
          <img alt="preuve csc 1" src="../assets/Lhoist_preuve.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuveIlu1" >
          <img alt="preuve csc 1" src="../assets/open_preuve.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuveIlu2" >
          <img alt="preuve csc 1" src="../assets/illustrator_preuve.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuveIlu3" >
          <img alt="preuve csc 1" src="../assets/illustrator_preuve_2.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuveNode1" >
          <img alt="preuve csc 1" src="../assets/open_preuve.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuveNode2" >
          <img alt="preuve csc 1" src="../assets/NodeJs_preuve.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuveNode3" >
          <img alt="preuve csc 1" src="../assets/NodeJs_preuve2.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuvePHP1" >
          <img alt="preuve csc 1" src="../assets/open_preuve.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuvePHP2" >
          <img alt="preuve csc 1" src="../assets/PHP_preuve1.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuvePHP3" >
          <img alt="preuve csc 1" src="../assets/PHP_preuve_2.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuveUTCTF1" >
          <img alt="preuve csc 1" src="../assets/UTCTF_preuve.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuveUTCTF2" >
          <img alt="preuve csc 1" src="../assets/UTCTF_preuve2.png" class="proof-img">
        </vs-dialog>
        <vs-dialog overflow-hidden not-close auto-width not-padding v-model="preuveGIMP" >
          <img alt="preuve csc 1" src="../assets/Attestation-Gimp.png" class="proof-img">
        </vs-dialog>
      </div>
    </div>
  </div>
</template>

<script>
    export default {
        name: "Portfolio",

      data(){
        return {
          actif1:false,
          actif2:false,
          actif3:false,
          actif4:false,
          actif5:false,
          actif6:false,
          actif7:false,
          actif8:false,
          preuveCSC1 :false,
          preuveCSC2 :false,
          preuveCSC3 :false,
          preuveLhoist:false,
          preuveIlu1 : false,
          preuveIlu2 : false,
          preuveIlu3 : false,
          preuveNode3: false,
          preuveNode2: false,
          preuveNode1 : false,
          preuvePHP1:false,
          preuvePHP2:false,
          preuvePHP3:false,
          preuveUTCTF1:false,
          preuveUTCTF2:false,
          preuveGIMP:false
        }
      }
    }
</script>

<style scoped>

  #title{
    text-align: center;
    font-family: Roboto,sans-serif;
    margin-bottom: 5%;
    font-weight: lighter;
    font-size: 220%;
    letter-spacing: 8px;
  }
  #main{
    margin-bottom: 10%;
  }
  .bold{
    font-weight: bold;
  }
  .logo{
    display: block;
    margin-right: auto;
    margin-left: auto;
    height: 80px;
    margin-bottom: 3%;
  }
  .dialog-title{
    font-size: 120%;
    margin-bottom: 2%;
  }
  .m4{
    margin-bottom: 4%;
  }
  .con-content{
    text-align: justify;
    font-size: 120%;
    height: 100%;
  }
  .con-content{
    margin-left: 3%;
    margin-right: 3%;
    text-align: justify;
  }
  .flex{
    display: flex;
    margin-top: 3%;
  }
  .preuve{
    flex: 1;
    margin-left: 8%;
    margin-right: 8%;
  }
  .proof-img{
    display: block;
    margin: auto;
    width: 800px;
  }
  .total {
    font-weight: bold;
    color: white;
    background-color: #072b43;
  }
  .row:hover{
    color: white;
    background-color: #072b43;
  }
  #tr{
    background-color: aliceblue;
  }
  #table{
    width: 100%;
  }
  #tableDiv{
    width: 75%;
    display: block;
    margin-right: auto;
    margin-left: auto;
  }
  .th{
    margin-left: 10%;
  }
  td{
    display: table-cell;
    padding-bottom: 1%;
    vertical-align: middle;
  }
</style>

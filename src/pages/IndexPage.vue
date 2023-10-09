<template>
  <q-page class="q-pa-md" style="background-color: #f9f7f7">
    <div class="row" data-aos="fade-right" data-aos-duration="2000">
      <div class="col-md-5 flex justify-center">
        <q-img
          class="photo"
          src="src\assets\moi.jpg"
          @mouseover="affichage = true"
          @mouseout="affichage = false"
        />
        <div class="informations" :class="{ visible: affichage }">
          <div>
            <q-icon name="mail" />
            regnierbpro62@gmail.com
          </div>
          <div>
            <q-icon name="call" />
            07 85 54 01 57
          </div>
          <div>
            <q-icon name="location_pin" />
            Lille (59), Hauts-de-France
          </div>
        </div>
      </div>
      <div
        class="col-md-7 q-gutter-y-md q-pa-md"
        style="color: #112d4e; text-align: justify"
      >
        <div class="title">Baptiste Régnier</div>
        <div style="font-size: 20px">
          Développeur web Full Stack en alternance<br />
          (2 semaines en entreprise/ 1 semaine de formation)
        </div>
        <div>
          Enthousiaste, passionné par le développement et la conception
          d'applications, je suis actuellement à la recherche d'une opportunité
          d'alternance qui me permettrait de concrétiser ma passion tout en
          continuant d'apprendre et de progresser dans le domaine. Mon modèle
          d'alternance est basé sur un cycle de 2 semaines en entreprise, suivi
          d'une semaine en école pour acquérir des connaissances nouvelles et
          appliquer ce que j'ai appris.
        </div>
        <div>
          Ma capacité à travailler en équipe est l'un de mes atouts majeurs. Je
          crois en la force de la collaboration et je suis à l'aise de partager
          des idées et des responsabilités pour atteindre des objectifs communs.
          En tant que développeur, je suis également créatif dans la recherche
          de solutions innovantes et je suis connu pour être consciencieux dans
          mon travail, veillant à la qualité et à la robustesse de chaque ligne
          de code que je produis.
        </div>
        <div>
          En somme, je suis impatient de rejoindre une entreprise dynamique où
          je pourrai mettre en pratique mes compétences tout en continuant
          d'apprendre et de grandir. Mon engagement envers le développement de
          qualité et ma volonté d'apporter une contribution significative font
          de moi un candidat idéal pour une alternance dans le domaine du
          développement et de la conception d'applications.
        </div>
      </div>
    </div>
    <div class="separateur" data-aos="fade-up" data-aos-duration="2000"></div>
    <div class="row" data-aos="fade-left">
      <div class="title full-width q-pb-lg">Compétences</div>
      <div class="col-md-4 flex justify-center">
        <q-img
          class="hardSkill"
          src="src\assets\html-5.png"
          @click="affichageCompetence1 = !affichageCompetence1"
        />
        <q-img
          class="hardSkill"
          src="src\assets\css-3.png"
          @click="affichageCompetence1 = !affichageCompetence1"
        />
        <q-card v-if="affichageCompetence1" class="full-width">
          <q-card-section>HTML CSS</q-card-section>
          <q-card-section>blabla</q-card-section>
        </q-card>
      </div>
      <div class="col-md-2 flex justify-center">
        <q-img
          class="hardSkill"
          src="src\assets\python.png"
          @click="affichageCompetence2 = !affichageCompetence2"
        />
        <q-card v-if="affichageCompetence2" class="full-width">
          <q-card-section>Python</q-card-section>
          <q-card-section>blabla</q-card-section>
        </q-card>
      </div>
      <div class="col-md-2 flex justify-center">
        <q-img
          class="hardSkill"
          src="src\assets\php.png"
          @click="affichageCompetence3 = !affichageCompetence3"
        />
        <q-card v-if="affichageCompetence3" class="full-width">
          <q-card-section>PHP</q-card-section>
          <q-card-section>blabla</q-card-section>
        </q-card>
      </div>
      <div class="col-md-2 flex justify-center">
        <q-img
          class="hardSkill"
          src="src\assets\quasar.png"
          @click="affichageCompetence4 = !affichageCompetence4"
        />
        <q-card v-if="affichageCompetence4" class="full-width">
          <q-card-section>Quasar</q-card-section>
          <q-card-section>blabla</q-card-section>
        </q-card>
      </div>
      <div class="col-md-2 flex justify-center">
        <q-img
          class="hardSkill"
          src="src\assets\vueJS.png"
          @click="affichageCompetence5 = !affichageCompetence5"
        />
        <q-card v-if="affichageCompetence5" class="full-width">
          <q-card-section>VueJS</q-card-section>
          <q-card-section>blabla</q-card-section>
        </q-card>
      </div>
    </div>
    <div class="separateur" data-aos="fade-up" data-aos-duration="2000"></div>
    <div class="row" data-aos="fade-right">
      <div class="title full-width q-pb-lg">Savoir être</div>
      <div class="col-md-4 flex justify-center">
        <div class="full-width flex justify-center">Consciencieux</div>
        <q-img class="softSkill" src="src/assets/consciencieux.jpg"></q-img>
      </div>
      <div class="col-md-4 flex justify-center">
        <div class="full-width flex justify-center">Créatif</div>
        <q-img class="softSkill" src="src/assets/creatif.jpg"></q-img>
      </div>
      <div class="col-md-4 flex justify-center">
        <div class="full-width flex justify-center">Travail d'équipe</div>
        <q-img class="softSkill" src="src/assets/travailEquipe.png"></q-img>
      </div>
    </div>
    <div class="separateur" data-aos="fade-up" data-aos-duration="2000"></div>

    <div
      class="row"
      data-aos="fade-right"
      data-aos-duration="2000"
      style="height: 800px"
    >
      <div class="title full-width q-pb-lg">Parcours</div>
      <div class="col-md-4 flex column justify-evenly">
        <div data-aos="fade-up" data-aos-duration="2000">
          HIVER 2023 - Lota.Cloud
        </div>
        <div data-aos="fade-up" data-aos-duration="2000">
          PRINTEMPS 2022 - YOOZLY
        </div>
        <div data-aos="fade-up" data-aos-duration="2000">2021</div>
        <div data-aos="fade-up" data-aos-duration="2000">2021</div>
      </div>
      <div class="ligne flex column justify-evenly">
        <div data-aos="fade-up" data-aos-duration="2000" class="point"></div>
        <div data-aos="fade-up" data-aos-duration="2000" class="point"></div>
        <div data-aos="fade-up" data-aos-duration="2000" class="point"></div>
        <div data-aos="fade-up" data-aos-duration="2000" class="point"></div>
      </div>
      <div class="col-md-7 flex column justify-evenly">
        <q-card
          data-aos="fade-up"
          data-aos-duration="2000"
          class="carteParcours"
        >
          <q-section>DEVELOPPEUR WEB (STAGIAIRE)</q-section>
          <q-separator />
          <q-section
            >Développement du nouveau siteweb à partir d'un maquette</q-section
          >
        </q-card>
        <q-card
          data-aos="fade-up"
          data-aos-duration="2000"
          class="carteParcours"
        >
          <q-section>DEVELOPPEUR WEB (STAGIAIRE)</q-section>
          <q-separator />
          <q-section
            >Participation aux activités dedéveloppement web de
            l'agence,résolution de tickets.</q-section
          >
        </q-card>
        <q-card
          data-aos="fade-up"
          data-aos-duration="2000"
          class="carteParcours"
        >
          <q-section>étudiant à l'EPSI</q-section>
          <q-separator />
          <q-section>
            <q-list>
              <q-item>développement web </q-item>
              <q-item>développement d’application</q-item>
              <q-item>gestion de base de donnée</q-item>
            </q-list>
          </q-section>
        </q-card>
        <q-card
          data-aos="fade-up"
          data-aos-duration="2000"
          class="carteParcours"
        >
          <q-section>BACCALAUREAT GENERAL</q-section>
          <q-separator />
          <q-section>
            <div>Spécialités :</div>
            <q-list>
              <q-item>Numérique et Sciences Informatique</q-item>
              <q-item
                >Langues, Littératures et Civ. étrangères (anglais)</q-item
              >
            </q-list>
          </q-section>
        </q-card>
      </div>
    </div>
  </q-page>
</template>

<script setup>
import { ref, onMounted } from "vue";
import AOS from "aos";
import "aos/dist/aos.css";
const affichage = ref(false);
const affichageCompetence1 = ref(false);
const affichageCompetence2 = ref(false);
const affichageCompetence3 = ref(false);
const affichageCompetence4 = ref(false);
const affichageCompetence5 = ref(false);
onMounted(() => {
  AOS.init();
});
</script>

<style>
.photo {
  width: 300px;
  height: 450px;
  border-radius: 30px;
}
.informations {
  display: none;
  position: absolute;
  width: 300px;
  height: 450px;
  background-color: #ffffff;
  color: #112d4e;
  padding: 10px;
  font-size: 16px;
}
.informations.visible {
  display: flex;
  border-radius: 30px;
  flex-direction: column;
  justify-content: space-evenly;
  opacity: 0.7;
  background-color: #000000;
  color: #f9f7f7;
}
.separateur {
  height: 3px;
  width: 40%;
  background-color: #3f72af;
  border-radius: 30px;
  margin: 100px auto;
}

.title {
  font-size: 60px;
  font-family: Arial, Helvetica, sans-serif;
  color: #112d4e;
  margin-top: -10px;
}
.hardSkill {
  width: 100px;
  height: 100px;
}
.softSkill {
  width: 200px;
  height: 200px;
}
.carteCompetence {
  position: absolute;
}
.carteParcours {
  width: 400px;
}
.ligne {
  background-color: #3f72af;
  width: 3px;
  border-radius: 30px;
  margin-right: 90px;
}
.point {
  width: 10px;
  height: 10px;
  border-radius: 30px;
  background-color: #3f72af;
}
</style>

<template>
  <div>
    <h1>Bienvenue sur mon site internet personnel.</h1>

    <v-carousel cycle height="400" show-arrows-on-hover interval="4000">
      <v-carousel-item v-for="(slide, i) in slides" :key="i" :src="slide.src">
        <v-row class="fill-height" align="center" justify="center">
          <div class="display-3">{{ slide.text }}</div>
        </v-row>
      </v-carousel-item>
    </v-carousel>

    <v-divider class="my-4"></v-divider>

    <h1>Présentation :</h1>
    <span>
      Ayant commencé sur Java, je travaille aujourd'hui dans l'écosystème
      JavaScript, avec Node.js et Vue.js.
    </span>
    <br />
    <span>SQL avec PostgreSQL, NoSQL avec MongoDB.</span>
    <v-spacer />

    <v-divider class="my-4"></v-divider>

    <h2>Compétences clés :</h2>
    <span>
      Travail en équipe. Avenant. Passionné. Autodidacte. Autonome.
      Anticipation. Organisation d'une équipe de travail. Veille technologique.
    </span>

    <v-divider class="my-4"></v-divider>

    <Experience></Experience>

    <v-divider class="my-4"></v-divider>

    <Formation></Formation>
  </div>
</template>

<script>
import Formation from "@/components/home/Formation.vue";
import Experience from "@/components/home/Experience.vue";

export default {
  name: "Home",
  components: {
    Formation,
    Experience,
  },
  data: () => ({
    slides: [
      {
        text: "Made with love and Vue.js",
        src:
          "https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/1200px-Vue.js_Logo_2.svg.png",
      },
      {
        text: "The place where I'm postings my works.",
        src:
          "https://images.idgesg.net/images/article/2019/02/certification_school_pencils_diversity_creative_team_by-evgeny555-getty-100787956-large.jpg",
      },
      {
        text: "Working on multiple languages and technologies.",
        src:
          "https://upload.wikimedia.org/wikipedia/commons/thumb/9/99/Unofficial_JavaScript_logo_2.svg/1200px-Unofficial_JavaScript_logo_2.svg.png",
      },
      {
        text: "Skill: Node.js",
        src:
          "https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Node.js_logo.svg/1200px-Node.js_logo.svg.png",
      },
      {
        text: "Language: Java",
        src:
          "https://upload.wikimedia.org/wikipedia/fr/thumb/2/2e/Java_Logo.svg/1200px-Java_Logo.svg.png",
      },
      {
        text: "Database: SQL & NoSQL",
        src:
          "https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/Postgresql_elephant.svg/1200px-Postgresql_elephant.svg.png",
      },
    ],
  }),
};
</script>
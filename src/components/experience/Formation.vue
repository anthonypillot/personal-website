<template>
  <div>
    <h1>Formation :</h1>
    <v-divider class="my-4"></v-divider>

    <v-col cols="12">
      <v-row>
        <v-card tile>
          <v-list disabled>
            <v-subheader>
              ÉCOLE D'INFORMATIQUE - 2018 / 2020
              <br />Bachelor - Titre professionnel RNCP - Concepteur Développeur
              d'Application
            </v-subheader>
            <v-list-item-group color="primary">
              <v-list-item v-for="skill in bachelorSkills" :key="skill.text">
                <v-list-item-content>
                  <v-list-item-title v-text="skill.text"></v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-list-item-group>
          </v-list>
        </v-card>

        <v-divider vertical class="ma-2" />

        <v-card tile>
          <v-list disabled>
            <v-subheader>
              UNIVERSITÉ DE LILLE III - CHARLES-DE-GAULLE - 2015 / 2018
              <br />LICENCE de Psychologie, parcours et spécialisation
              Psychologie du Travail.
            </v-subheader>
            <v-list-item-group color="primary">
              <v-list-item v-for="skill in licenceSkills" :key="skill.text">
                <v-list-item-content>
                  <v-list-item-title v-text="skill.text"></v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-list-item-group>
          </v-list>
        </v-card>
      </v-row>
    </v-col>
  </div>
</template>

<script>
export default {
  name: "Formation",
  data: () => ({
    bachelorSkills: [
      {
        text: "Java, JavaFX, JEE.",
      },
      {
        text: "Hibernate.",
      },
      {
        text: "Microsoft SQL Server, PostgreSQL.",
      },
      {
        text: "HTML5, CSS3, JavaScript.",
      },
      {
        text:
          "Et d'autre technologies : Node.js, Kotlin, Talend Data Integration.",
      },
    ],
    licenceSkills: [
      {
        text: "Psychologie du travail.",
      },
      {
        text: "Psychologie des organisations.",
      },
      {
        text: "Psychologie des inégalités et de l'intégration au travail.",
      },
      {
        text: "Étude des relations sociales au travail.",
      },
      {
        text: "Gestion des risques psychosociaux.",
      },
      {
        text: "Étude des Ressources Humaines.",
      },
    ],
  }),
};
</script>

<style></style>

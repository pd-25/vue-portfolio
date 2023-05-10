<template>
  <v-container>
    <v-row justify="center">
      <v-col lg="12" class="text-center">
        <v-subheader class="text-h4 justify-center"> Some of my work</v-subheader>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus, rerum.</p>
      </v-col>

      <v-col lg="12">
        <div class="text-center">
          <v-chip
            @click="activeChip = 'webApplication'"
            :color="activeChip == 'webApplication' ? 'success' : ''"
            class="mx-4"
            >Web Applications</v-chip
          >
          <v-chip
            @click="activeChip = 'leetCode'"
            :color="activeChip == 'leetCode' ? 'success' : ''"
            class="mx-4"
            >Leetcode
          </v-chip>
          <v-chip
            @click="activeChip = 'youTube'"
            :color="activeChip == 'youTube' ? 'success' : ''"
            class="mx-4"
            >Youtube</v-chip
          >
        </div>
      </v-col>

      <slot v-if="activeChip == 'webApplication'">
        <v-col lg="3" v-for="(webApp, webIndex) in webApplications" :key="webIndex">
          <a href="https://mail.google.com/mail/u/0/#inbox" target="_blank">
            <v-card>
              <v-img
                :src="webApp.image"
                class="white-text align-end"
                gradient="to buttom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                height="200px"
              >
                <v-card-title>{{ webApp.title }}</v-card-title>
              </v-img>
            </v-card>
          </a>
        </v-col>
      </slot>

      <slot v-if="activeChip == 'leetCode'">
        <v-col lg="3" v-for="(leetCode, leetCodeIndex) in leetCodes" :key="leetCodeIndex">
          <a href="https://mail.google.com/mail/u/0/#inbox" target="_blank">
            <v-card>
              <v-img
                :src="leetCode.image"
                class="white-text align-end"
                gradient="to buttom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                height="200px"
              >
                <v-card-title>{{ leetCode.title }}</v-card-title>
              </v-img>
            </v-card>
          </a>
        </v-col>
      </slot>

      <slot v-if="activeChip == 'youTube'">
        <v-col lg="3" v-for="(youTube, youTubeIndex) in youTubes" :key="youTubeIndex">
          <a href="https://mail.google.com/mail/u/0/#inbox" target="_blank">
            <v-card>
              <v-img
                :src="youTube.image"
                class="white-text align-end"
                gradient="to buttom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                height="200px"
              >
                <v-card-title>{{ youTube.title }}</v-card-title>
              </v-img>
            </v-card>
          </a>
        </v-col>
      </slot>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "PortfolioComp",

  data() {
    return {
      activeChip: "webApplication",
      webApplications: [
        { title: "Web App 1", image: "../src/assets/img/slides-3.jpg" },
        { title: "Web App 2", image: "../src/assets/img/slides-1.jpg" },
        { title: "Web App 3", image: "../src/assets/img/slides-2.jpg" },
        { title: "Web App 4", image: "../src/assets/img/news-1.jpg" },
        { title: "Web App 5", image: "../src/assets/img/news-2.jpg" },
      ],

      leetCodes: [
        { title: "leetCode 1", image: "../../src/assets/img/slides-3.jpg" },
        { title: "leetCode 2", image: "../src/assets/img/slides-1.jpg" },
        { title: "leetCode 3", image: "../src/assets/img/slides-2.jpg" },
        { title: "leetCode 4", image: "../src/assets/img/news-1.jpg" },
        { title: "leetCode 5", image: "../src/assets/img/news-2.jpg" },
      ],

      youTubes: [
        { title: "Fitness Channel", image: "../src/assets/img/slides-3.jpg" },
        { title: "Vlogging Channel", image: "../src/assets/img/slides-1.jpg" },
      ],
    };
  },
};
</script>

<style scoped>
.v-card-title {
  color: #ffffff;
}
</style>

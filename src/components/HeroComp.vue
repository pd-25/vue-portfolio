<template>
  <v-container class="pt-15" id="home">
    <v-row>
      <v-col lg="6">
        <h2 class="intro-text">Hi friends, welcome to my portfolio</h2>
        <p class="description">
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quis nemo similique
          accusantium impedit laborum quaerat voluptas hic eum? Totam aliquam aperiam ab
          sed vero beatae laudantium tempore dolore in ad!
        </p>
        <v-btn color="success" class="white-text mr-10" rounded>Get Started</v-btn>
        <v-btn color="primary" class="white-text" rounded>
          <v-icon>mdi-play-circle</v-icon>Watch Video
        </v-btn>
      </v-col>
      <v-col lg="6">
        <v-img width="100%" height="80%" src="../src/assets/img/pd.jpg"></v-img>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
h2.intro-text {
  font-size: 55px;
  font-weight: bold;
  font-family: sans-serif;
  color: #444;
}

p.description {
  font-size: 19;
  font-family: sans-serif;
  margin: 32px 0px;
  color: #444444ba;
}

.v-img {
  border-radius: 50%;
}
</style>

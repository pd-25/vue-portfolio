<template>
  <v-container class="my-5">
    <v-row justify="center">
      <v-col lg="12" class="text-center">
        <v-subheader class="text-h4 justify-center"> Projects</v-subheader>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus, rerum.</p>
      </v-col>
      <v-col lg="4" v-for="(project, projectIndex) in 3" :key="projectIndex">
        <v-card class="mx-auto my-5" max-width="374">
          <v-img height="250" src="../src/assets/img/slides-3.jpg"></v-img>
          <v-card-title>Web development</v-card-title>
          <v-card-text>
            <div>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores, sequi!
            </div>
          </v-card-text>
          <v-divider class="mx-4"></v-divider>
          <v-card-action class="d-flex py-3">
            <v-btn color="success" rounded>View Details</v-btn>
            <v-spacer></v-spacer>
            <v-rating
              :value="4.5"
              color="amber"
              dense
              half-increments
              readonly
              size="25"
            ></v-rating>
          </v-card-action>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

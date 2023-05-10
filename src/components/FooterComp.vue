<template>
  <v-footer class="text-center">
    <v-col lg="12">
      <v-row justify="center">
        <v-col lg="4">
          <v-toolbar-title
            ><span class="text-success">Pradipta</span> S Bhuin
          </v-toolbar-title>
          <div>
            <v-btn
              v-for="icon in icons"
              :key="icon"
              class="mx-4"
              :icon="icon"
              variant="text"
            ></v-btn>
          </div>
        </v-col>
      </v-row>
      <v-subheader
        >Thanks For Visiting My Portfolio, This Postfolio is Build in VueJs &
        Vuetify</v-subheader
      >
      <v-divider class="mt-2"></v-divider>
      <v-subheader class="mt-2 d-flex">
        <div>{{ new Date().getFullYear() }} — <strong>Vuetify</strong></div>
        <v-spacer></v-spacer>
        <p>
          Designed By <strong><span class="text-success">Pradipta</span> S Bhuin </strong>
        </p>
      </v-subheader>
    </v-col>

    <v-divider></v-divider>
  </v-footer>
</template>

<script>
export default {
  data: () => ({
    icons: ["mdi-facebook", "mdi-twitter", "mdi-linkedin", "mdi-instagram"],
  }),
};
</script>

<template>
  <v-container>
    <v-row class="d-flex">
      <v-col lg="6">
        <v-img width="100%" height="80%" src="../src/assets/img/pd.jpg"></v-img>
      </v-col>

      <v-col lg="6">
        <v-subheader class="text-h4">Know me</v-subheader>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Doloribus repudiandae
          numquam quam aut, totam inventore, rem magni eveniet vero nesciunt reiciendis
          obcaecati libero? Distinctio officia et quos eveniet quod nisi?
        </p>
        <v-list>
          <v-list-item>
            <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
            <v-list-item-subtitle
              >Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus
              deleniti vel pariatur veritatis qui repellat cum. Voluptatibus illo ab dicta
              architecto quae consequuntur aut accusamus saepe, incidunt quisquam placeat
              veritatis?</v-list-item-subtitle
            >
          </v-list-item>

          <v-list-item>
            <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
            <v-list-item-subtitle
              >Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus
              incidunt quisquam placeat veritatis?</v-list-item-subtitle
            >
          </v-list-item>

          <v-list-item>
            <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
            <v-list-item-subtitle
              >Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </v-list-item-subtitle>
          </v-list-item>

          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nisi necessitatibus
            itaque quae illum vel molestias alias ea odit eaque voluptatem id impedit
            facere fugit non, obcaecati dicta, natus error fuga dolores dolore.
            Accusantium, quam ipsa voluptatibus dolor architecto ipsum placeat.
          </p>
        </v-list>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "AboutmeComp",
};
</script>

<style scoped>
.v-img {
  border-radius: 50%;
}
</style>

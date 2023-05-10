<template>
  <HeaderComp />
</template>

<script>
import { defineComponent } from "vue";

// Components
import HelloWorld from "../components/HelloWorld.vue";
import HeaderComp from "../components/HeaderComp.vue";

export default defineComponent({
  name: "HomeView",

  components: {
    HelloWorld,
    HeaderComp,
  },
});
</script>

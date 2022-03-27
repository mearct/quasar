<template>
  <q-layout view="hHh lpR fFf">
    <Header />

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer elevated class="bg-grey-8 text-white">
      <Footer />
    </q-footer>
  </q-layout>
</template>

<script>
import Header from "components/Header.vue";
import Footer from "components/Footer.vue";
export default {
  name: "FrontendLayout",
  components: {
    Header,
    Footer,
  },
  setup() {
    return {};
  },
};
</script>

<template>
  <q-header elevated class="bg-primary text-white" height-hint="98">
    <q-toolbar>
      <q-btn dense flat round icon="menu" @click="toggleLeftDrawer" />

      <q-toolbar-title>
        <q-avatar>
          <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg" />
        </q-avatar>
        Title
      </q-toolbar-title>

      <q-btn dense flat round icon="menu" @click="toggleRightDrawer" />
    </q-toolbar>
    <Navbar />
  </q-header>

  <q-drawer show-if-above v-model="leftDrawerOpen" side="left" bordered>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
  </q-drawer>

  <q-drawer show-if-above v-model="rightDrawerOpen" side="right" bordered>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
    <p>drawer content</p>
  </q-drawer>
</template>

<script>
import Navbar from "components/Navbar.vue";
import { ref } from "vue";
export default {
  name: "Header",
  components: {
    Navbar,
  },

  setup() {
    const leftDrawerOpen = ref(false);
    const rightDrawerOpen = ref(false);
    return {
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value;
      },

      rightDrawerOpen,
      toggleRightDrawer() {
        rightDrawerOpen.value = !rightDrawerOpen.value;
      },
    };
  },
};
</script>

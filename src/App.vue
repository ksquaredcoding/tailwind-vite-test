<template>

  <section class="h-full w-screen">

    <header>
      <NavBar class="h-screen left-0 w-1/5" />
    </header>
    <main>
      <RouterView />
    </main>
    <footer>
    </footer>
  </section>
  <TestModal />
</template>

<script>
import { computed } from 'vue'
import { AppState } from './AppState'
import NavBar from "./components/NavBar.vue";
import TestModal from "./components/TestModal.vue";
import { router } from './router'

export default {
  setup() {
    return {
      appState: computed(() => AppState)
    };
  },
  components: { NavBar, TestModal }
}
</script>
<style>
@import "style.css";


main {
  overflow: hidden;
  max-height: 100vh;
}

.nav-left {
  position: absolute;
  left: 0;
  top: 0;
  height: 100vh;
}
</style>

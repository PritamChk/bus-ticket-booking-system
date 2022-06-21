<template>
  <div class="h-screen w-full flex flex-col">
    <NavBar></NavBar>
    <router-view></router-view>
  </div>
</template>

<script>
import NavBar from "./components/Navbar.vue";
export default {
  components: {
    NavBar,
  },
  data() {
    return {};
  },
};
</script>

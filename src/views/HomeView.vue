<template>
  <div class="h-screen">
    <BusVue />
  </div>
</template>

<script>
import BusVue from "../components/Bus.vue";
export default {
  components: {
    BusVue,
  },
  data() {
    return {
      test: "hi",
    };
  },
};
</script>

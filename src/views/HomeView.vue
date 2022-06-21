<template>
  <div class="h-screen grid grid-flow-col grid-cols-2">
    <BusVue class="col-span-1" />
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

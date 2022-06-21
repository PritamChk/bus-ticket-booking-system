<template>
  <div class="h-screen grid grid-flow-col grid-cols-2">
    <BusVue class="col-span-1" />
    <BookingDetailBoxVue />
  </div>
</template>

<script>
import BusVue from "../components/Bus.vue";
import BookingDetailBoxVue from "../components/BookingDetailBox.vue";
export default {
  components: {
    BusVue,
    BookingDetailBoxVue,
  },
  data() {
    return {
      test: "hi",
    };
  },
};
</script>

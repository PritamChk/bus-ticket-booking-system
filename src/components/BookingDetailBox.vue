<template>
  <div
    class="border-2 text-lg bg-zinc-200 rounded-md mx-2 my-5 flex flex-col h-full"
  >
    <form action="#" @submit.prevent="doSomething">
      <section>
        <div>
          <label for="from">From</label>
          <select name="startLocation" id="SL-1">
            <template
              v-for="(startLocation, index) in startLocations"
              :key="index"
            >
              <option value="">{{ index + 1 }} . {{ startLocation }}</option>
            </template>
          </select>
        </div>
        <div>
          <label for="To">To</label>
          <select name="stoppageLocation" id="SR-1">
            <template
              v-for="(stoppageLoc, index) in stoppageLocations"
              :key="index"
            >
              <option value="">{{ index + 1 }} . {{ stoppageLoc }}</option>
            </template>
          </select>
          <section>
            <div>
              <label for="date">Date</label>
              <input type="date" />
            </div>
            <div>
              <label for="date">Time Slot</label>
              <input type="time" />
            </div>
          </section>
        </div>
      </section>
    </form>
  </div>
</template>

<script>
import { Menu, MenuButton, MenuItems, MenuItem } from "@headlessui/vue";
import { ChevronDownIcon } from "@heroicons/vue/solid";

export default {
  name: "BookingDetailBox",
  created() {},
  data() {
    return {
      startLocations: ["Esplaned", "Maidan", "Exide"],
      stoppageLocations: [
        "Park Street",
        "Maidan",
        "Esplaned",
        "Dharmatala",
        "Wellington",
        "Shealdah",
      ],
    };
  },
  props: {},
  methods: {
    doSomething() {
      console.log("Form Submitted");
    },
  },
};
</script>

<style lang="scss" scoped></style>

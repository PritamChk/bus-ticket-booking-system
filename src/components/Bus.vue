<template>
  <section
    class="rounded-lg shadow-md h-9/12 w-3/6 bg-zinc-200 mx-auto my-10 flex flex-col"
  >
    <header class="flex flex-row justify-between items-center h-44">
      <h1
        class="border-r-2 rounded-xl border-t-2 border-b-2 px-10 py-10 border-gray-800/30 text-2xl"
      >
        Entry
      </h1>
      <h1
        class="border-2 rounded-xl mr-3 px-10 py-10 border-gray-800/30 text-2xl"
      >
        Driver
      </h1>
    </header>
    <main class="grid grid-cols-5 gap-1 grid-flow-col">
      <section class="col-span-2 grid grid-cols-2 grid-rows-5">
        <template v-for="Lseat in L1">
          <button
            class="w-16 h-16 bg-gray-500 mx-2 my-2 rounded-lg col-span-1 row-span-1"
          >
            {{ Lseat }}
          </button>
        </template>
      </section>
      <div class="col-span-1 border-l-2 border-r-2 border-gray-700">
        <div
          class="-rotate-90 text-xl font-semibold font-mono transform-gpu flex flex-row justify-center items-center h-full"
        >
          <span>Passage</span>
        </div>
      </div>
      <section class="col-span-2 grid grid-cols-2 grid-rows-5">
        <template v-for="Rseat in R1">
          <button
            class="w-16 h-16 bg-gray-500 mx-2 my-2 rounded-lg col-span-1 row-span-1"
          >
            {{ Rseat }}
          </button>
        </template>
      </section>
    </main>
  </section>
</template>
<script>
export default {
  name: "BusView",
  data() {
    return {
      L1: 10,
      R1: 10,
    };
  },
};
</script>

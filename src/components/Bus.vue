<template>
  <section
    class="rounded-lg shadow-lg bg-zinc-300 mx-auto my-10 flex flex-col"
  >
    <header class="flex flex-row justify-between items-center h-44">
      <h1
        class="border-r-2 rounded-r-xl border-t-2 border-b-2 px-10 py-10 border-gray-800/30 text-2xl"
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
            class="hover:bg-sky-200 slow text-lg font-medium cursor-pointer w-16 h-16 shadow-md shadow-zinc-600/20 bg-gray-100 mx-2 my-3 rounded-lg col-span-1 row-span-1"
          >
            L{{ Lseat }}
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
      <section class="col-span-2 grid grid-cols-2 grid-rows-5 gap-1">
        <template v-for="Rseat in R1">
          <button
            class="hover:bg-sky-200 slow text-lg font-medium cursor-pointer w-16 h-16 shadow-zinc-600/20 bg-gray-100 shadow-md mx-2 my-3 rounded-lg col-span-1 row-span-1"
          >
            R{{ Rseat }}
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
      L1: 12,
      R1: 12,
    };
  },
};
</script>

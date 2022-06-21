<template>
  <nav
    class="w-full text-gray-100 flex flex-row flex-wrap justify-around items-center py-3 text-lg font-bold bg-gray-900/70 backdrop-filter backdrop-blur-md sticky top-0"
  >
    <div>logo</div>
    <ul>
      <li>
        <router-link :to="{ name: 'home' }">Home</router-link>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
};
</script>

<style lang="scss" scoped></style>

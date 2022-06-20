<template>
  <nav>
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

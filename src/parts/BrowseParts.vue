<template>
  <div>
    <h1>Browse Parts</h1>
    <ul class="menu">
      <li>
        <router-link :to="{ name: 'BrowseHeads', params: {} }">Heads</router-link>
      </li>
      <router-link :to="{ name: 'BrowseArms', params: {} }">Arms</router-link>
      <router-link :to="{ name: 'BrowseTorsos', params: {} }">Torsos</router-link>
      <router-link :to="{ name: 'BrowseBases', params: {} }">Bases</router-link>
    </ul>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'BrowseParts',
};
</script>

<style scoped>
  h1 {
    text-align: center;
  }
  .menu {
    display: flex;
    justify-content: space-around;
    margin: 0 100px;
    font-size: 20px;
  }
  ul {
    list-style-type: none;
  }
  a {
    color: palevioletred;
  }
</style>

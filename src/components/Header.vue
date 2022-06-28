<template>
  <header>
    <h1><a v-bind:href="'/Home'">POKA</a></h1>
      <!--<router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>-->
  </header>
</template>

<script>

export default {
  name: 'Header',
  props: {
    title: String,
  },
  components: {
  },
}
</script>

<style lang="scss">
  header {
    display: flex;
    align-items: center;
    justify-content: center;
    position: fixed;
    padding: 0px 50px;

    h1{
      a {
      font-size: 100px;
      text-transform: capitalize;
      mix-blend-mode: difference;
      }
    }

  }
/*
  h1 {
    font-style: $logo-font-family;
    
  }
*/
</style>
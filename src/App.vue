<template>
  <div class="container">  
    <Header />
    <MainSection />
    <SidebarLeft />
    <SidebarRight />
    <CursorCircle />
  </div>
</template>

<script>
import Header from './components/Header'
import SidebarLeft from './components/SidebarLeft'
import SidebarRight from './components/SidebarRight'
import CursorCircle from './components/CursorCircle'
import MainSection from './components/MainSection'


export default {
  name: 'App',
  components: {
    Header,
    SidebarLeft,
    SidebarRight,
    CursorCircle,
    MainSection,
  },
  methods: {
  }
}
</script>

<style lang="scss">
@import "./main.scss";

body {
  background-color: lightgrey;
  min-height: 100vh;
  margin: 0;

}
#app {
  font-family: 'Assistant', 'Roboto', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.conatiner {
  position: relative;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
      }

    }
  
}

</style>

<template>
  <div id="app">
    <Header
    :NavList="NavList"
    />
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header,
  },
  data () {
    return {
      NavList: [
        "HOME",
        "ABOUT",
        "SERVICES",
        "PROCESS",
        "TEAM",
        "BLOG",
        "GET IN TOUCH",
      ],
    }
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  border: 0;
  padding: 0;
  box-sizing: border-box;
}

a {
  text-decoration: none;
  color: inherit;
}

ul {
  list-style-type: none;
}
  // @import '~@fortawesome/fontawesome-free/css/all.min.css';
</style>

<template>
  <div id="app">
    <Header />
    <Maincontent />
  </div>
</template>

<script>
import Header from './components/Header.Vue'
import Maincontent from './components/Maincontent.Vue'

export default {
  name: 'App',
  components: {
    Header,
    Maincontent
  },
}
</script>

<style lang="scss">

</style>

<template>
  <div id="app">
    <Header />
    <Jumbo />
    <Maincontent />
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Jumbo from '@/components/Jumbo.vue'
import Maincontent from '@/components/Maincontent.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'App',

  components: {
    Header,
    Maincontent,
    Jumbo,
    Footer,
  },
}
</script>

<style lang="scss">

@import "@/style/variables.scss";

</style>

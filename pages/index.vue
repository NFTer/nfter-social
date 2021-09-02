<template>
  <section class="container">
    <Sidebar />
    <section class="codeart-container">
      <Header />
      <Content />
      <Footer />
    </section>
  </section>
</template>

<script>
import { mapState } from 'vuex'
import { isEmptyAddress } from '@/utils/index'
import Sidebar from '@/components/NFT/Sidebar.vue'
import Header from '@/components/NFT/Header.vue'
import Content from '@/components/NFT/Content.vue'
import Footer from '@/components/NFT/Footer.vue'
export default {
  components: {
    Sidebar,
    Header,
    Content,
    Footer
  },
  computed: {
    ...mapState(['token']),
    noToken() {
      return isEmptyAddress(this.token.tokenAddress)
    }
  },
  methods: {}
}
</script>

<style lang="less">
.codeart-container {
  flex-direction: column;
  display: flex;
  flex: 1;
  flex-basis: auto;
  box-sizing: border-box;
  min-width: 0;
}
.container {
  display: flex;
  flex-direction: row;
  flex: 1;
  flex-basis: auto;
  box-sizing: border-box;
  min-width: 0;
  height: 100vh;
  width: 100vw;
}
</style>

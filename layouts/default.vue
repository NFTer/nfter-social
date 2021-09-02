<template>
  <div class="codeart">
    <nuxt />
  </div>
</template>

<script>
// import { mapState } from 'vuex'

// import AuthModal from '@/components/Auth/index.vue'
export default {
  name: 'Default',
  components: {
    // AuthModal
  },
  computed: {
    // ...mapState(['loginModalType', 'loginModalTitle']),
    // loginModalShow: {
    //   get() {
    //     return this.$store.state.loginModalShow
    //   },
    //   set(v) {
    //     this.$store.commit('SET_LOGIN_MODAL_SHOW', v)
    //   }
    // }
  }
}
</script>
<style lang="less">
html, body {
  padding: 0;
  margin: 0;
}
.codeart {
  background: #e9e6e4;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>

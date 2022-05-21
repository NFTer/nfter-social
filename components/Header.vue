<template>
  <header id="site-header">
    <section class="header-banner component row">
      <a
        class="header-logo"
        title="Home"
        href="/"
      >
        <div class="logo image" />
      </a>
      <a class="header-banner-main" href="/">
        <p />
        <!-- <p class="date" data-widget="date">
              <span class="day">Thursday,</span>
              <span class="month">May 7,</span>
              <span class="year">2020</span>
            </p> -->
        <h1 class="site-title">
          <span class="site-logo"><span class="nft-title">NFTer</span>
          </span>
          <span class="screenreader">NFTer</span>
        </h1>
        <h2 class="site-description">A social platform based on NFT</h2>
      </a>
      <!-- <Web3Status /> -->
      <div class="header-location">
        <button class="status-button disabled" disabled>
          <span>🚀 Launch App</span>
        </button>
      </div>
    </section>
    <nav class="main-menu nav-main">
      <div class="menu-main-menu-container">
        <ul id="menu-main-menu" class="menu">
          <li class="header-link">
            <a
              class="menu-item menu-item-type-post_type menu-item-object-page"
              :class="{ 'current-menu-item': page === 'about' }"
              target="_blank"
              href="https://docs.nfter.social/"
            >
              📖 {{ $t("docs") }}<span class="hover-indicator">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="-2 -4 150.93 80.58"
                  class="circle-1"
                >
                  <path
                    class="hover-path"
                    fill="none"
                    stroke="#26498d"
                    stroke-miterlimit="10"
                    stroke-width="15px"
                    d="M51.36,8.75q-9.14-.64-18.3-.85-4.92-.16-9.85,0c-3.22.23-6.62.7-9.39,2.49A21.08,21.08,0,0,0,8,16.62,17.68,17.68,0,0,0,5.8,21.85c-.68,2.42-1.13,4.43-.48,6.94,1,3.79,3.48,7,6,9.91a60.49,60.49,0,0,0,15,12.44C33.6,55.43,41.8,57.88,49.91,60a144.68,144.68,0,0,0,27.72,4.25c10.65.62,21.78.65,32.27-1.6a48.14,48.14,0,0,0,10.86-3.49,16.81,16.81,0,0,0,6-4.33,11,11,0,0,0,1.91-9.37c-1.11-5.29-4.53-9.43-8.55-12.91a71.43,71.43,0,0,0-17.8-10.19Q89.91,17.05,77.08,13C66.09,9.53,54.58,6,43,5.14a32.64,32.64,0,0,0-8.67.34"
                  />
                </svg> </span></a>
          </li>
          <li class="header-link">
            <a
              class=" menu-item menu-item-type-post_type menu-item-object-page"
              :class="{ 'current-menu-item': page === 'tokens' }"
              target=""
              href="#roadmap"
            >
              🚌 {{ $t("roadMap") }}<span class="hover-indicator">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 414.84 111.47"
                  class="circle-2"
                >
                  <path
                    fill="none"
                    stroke="#26498d"
                    stroke-miterlimit="10"
                    stroke-width="25px"
                    class="hover-path"
                    d="M180.35,13.55c34.13-1.2,68.69-2.81,102.4,4.3,16.68,3.52,34,8,42.07,24.47,6.87,14.12.21,30.15-13.29,37-14.74,7.47-31.66,8.88-47.81,10.7-37.22,4.19-74.64,6.71-112.06,8.23-26.8,1.09-53.5,1-80.27-.54q-13.88-.54-27.64-2.36a52.37,52.37,0,0,1-16.92-3.74,26.59,26.59,0,0,1-13.5-18.42c-1.42-6.8-1.45-11.7,3.62-16.94,10.74-11.1,28.44-15.61,42.88-20.07a334.43,334.43,0,0,1,58.34-10q39.16-5.09,78.66-6.47c49.34-2.31,98.76-1.35,148.06,1.27,19.22,1,38.35,2.18,57.45,4.55"
                  />
                </svg> </span></a>
          </li>
          <li class="header-link">
            <a
              class="menu-item menu-item-type-post_type menu-item-object-page"
              :class="{ 'current-menu-item': page === 'trade' }"
              target=""
              href="#faq"
            >
              🙋 {{ $t("FAQ") }}<span class="hover-indicator">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 394.1 152.8"
                  class="circle-3"
                >
                  <path
                    fill="none"
                    stroke="#26498d"
                    stroke-miterlimit="10"
                    stroke-width="30px"
                    class="hover-path"
                    d="M104.1,58.5c-25.8,0.1-54.1,3.7-75,20.2c-6.4,5-11.8,11-13.7,19.1c-2.3,9.3,5.9,20.1,13,24.8
                c14.3,9.3,31.5,10.9,48,12.5c36.1,3.7,72.4,3,108.6,1.3c25-1.1,49.9-3.6,74.7-7.4c21.3-2.2,42.4-6.3,63-12.2
                c9.3-3.2,18.6-6.4,27.9-9.6c11-2.4,19.7-8,26.2-16.8c-4.6-10.3-12.3-17.4-23.1-21.2c-17.4-11.4-36.1-20.4-55.9-27
                c-33.5-12.8-71.9-23.1-108-25.8c-17.8-1.3-37.2-2.9-54.7,1.4c-5.4,1.3-11.6,2.5-14.6,7.7"
                  />
                </svg> </span></a>
          </li>
          <li class="header-link">
            <a
              class=" menu-item menu-item-type-post_type menu-item-object-page"
              :class="{ 'current-menu-item': page === 'issue' }"
              target=""
              href="#team"
            >
              🧘 {{ $t("team") }}<span class="hover-indicator">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="-2 -4 150.93 80.58"
                  class="circle-1"
                >
                  <path
                    class="hover-path"
                    fill="none"
                    stroke="#26498d"
                    stroke-miterlimit="10"
                    stroke-width="15px"
                    d="M51.36,8.75q-9.14-.64-18.3-.85-4.92-.16-9.85,0c-3.22.23-6.62.7-9.39,2.49A21.08,21.08,0,0,0,8,16.62,17.68,17.68,0,0,0,5.8,21.85c-.68,2.42-1.13,4.43-.48,6.94,1,3.79,3.48,7,6,9.91a60.49,60.49,0,0,0,15,12.44C33.6,55.43,41.8,57.88,49.91,60a144.68,144.68,0,0,0,27.72,4.25c10.65.62,21.78.65,32.27-1.6a48.14,48.14,0,0,0,10.86-3.49,16.81,16.81,0,0,0,6-4.33,11,11,0,0,0,1.91-9.37c-1.11-5.29-4.53-9.43-8.55-12.91a71.43,71.43,0,0,0-17.8-10.19Q89.91,17.05,77.08,13C66.09,9.53,54.58,6,43,5.14a32.64,32.64,0,0,0-8.67.34"
                  />
                </svg> </span></a>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>
<script>
// import Web3Status from './Web3Status'
import consts from '@/utils/consts'
export default {
  components: {
    // Web3Status
  },
  data() {
    return {
      page: '',
      uniswapURL: consts.uniswapURL
    }
  },
  computed: {
  },
  mounted() {
    this.page = this.$route.name
  },
  methods: {
  }
}
</script>

<style lang="less" scoped>
.header-logo .logo {
  background-image: url(../assets/logo_icon.png);
  background-size: 50%;
}
a.current-menu-item {
  color: #26498d;
  .hover-indicator {
    stroke-dashoffset: 0;
    opacity: 1;
  }
}
.nft-title {
  color: #26498d;
  background-image: -webkit-linear-gradient(right, #6055a2, #5964a5
, #5078a9);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.status-button {
  display: flex;
  width: 100%;
  font-size: 0.9rem;
  align-items: center;
  box-sizing: border-box;
  cursor: pointer;
  user-select: none;
  background-color: #fffcf9;
  font-weight: 400;
  flex-flow: row nowrap;
  padding: 1rem;
  border: 2px solid #231f20;
  &:hover {
    background-color: rgb(242, 242, 242);
    color: #26498d;
  }
  span {
    text-overflow: ellipsis;
    white-space: nowrap;
    font-size: 1.4rem;
    flex: 1 1 auto;
    overflow: hidden;
    margin: 0;
    font-weight: 700;
  }
  .section-heading {
    font-size: 1rem;
  }
}
/* .image{
  filter:brightness(90%) grayscale(100%) contrast(130%);transition:filter .9s;
  -webkit-user-drag:none;
  user-drag:none;
  &:hover {
    filter:brightness(100%) grayscale(0) contrast(100%);
  }
} */
</style>

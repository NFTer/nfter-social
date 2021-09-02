<template>
  <aside class="codeart-aside">
    <div class="logo">
      <img src="@/assets/images/code.png" alt="">
    </div>
    <div class="socialMediaContainer">
      <a role="button" aria-label="Discord" href="https://bit.ly/3aSYvPA" target="_blank">
        <img src="@/assets/images/Discord.svg" alt="">
      </a>
      <a role="button" aria-label="Twitter" href="https://twitter.com/rss3_" target="_blank">
        <img src="@/assets/images/Twitter.svg" alt="">
      </a>
    </div>
  </aside>
</template>

<style lang="less" scoped>
.codeart-aside {
  text-align: center;
  color: #333;
  overflow: auto;
  box-sizing: border-box;
  flex-shrink: 0;
  background-color: #fff;
  border: 1px solid #000;
  width: 12%;
  min-width: 90px;
  max-width: 170px;
  position: relative;
}
.logo {
  padding: 20%;
  display: flex;
  img {
    width: 100%;
  }
}

.socialMediaContainer {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  align-items: center;
  cursor: pointer;
  position: absolute;
  bottom: 0;
  width: 100%;
  padding: 20%;
  box-sizing: border-box;
  a {
    display: block;
    padding: 20%;
  }
}
</style>

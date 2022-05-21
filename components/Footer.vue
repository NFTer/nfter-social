<template>
  <div class="footer-items component row">
    <div class="footer-item footer-copy col-12 col-sm-4">
      Copyright © 2022 NFTer Labs 💡
      <!-- ©2018 SEA HARVEST AUSTRALIA, FRESH SEAFOOD MARKET -->
    </div>
    <div class="footer-item footer-copy col-12 col-sm-4">
      / <a href="#" class="disabled">Twitter</a> /
      <a href="#" class="disabled">Telegram</a> /
      <a href="https://github.com/nfter">Github</a> /
    </div>
    <!-- <a
      href=""
      class="footer-item footer-locations col-12 col-sm-4 uppercase"
    >
      Twitter / Telegram / Wechat
    </a> -->
    <div class="footer-item footer-copy col-12 col-sm-4">
      🌎 <a :href="$i18n.locale !== 'en' ? $route.fullPath.replace(/^\/[^\/]+/, '') : $route.fullPath">English</a> /
      <a :href="$i18n.locale !== 'zh'?`/zh` + $route.fullPath:$route.fullPath">中文</a>
    </div>

    <!-- <a
      href="https://www.ed.com.au/"
      target="_blank"
      class="footer-item footer-ed col-12 col-sm-4"
    >
      WEBSITE BY ED.
    </a> -->
  </div>
</template>
<style>

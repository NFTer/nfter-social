<template>
  <div class="component row">
    <div class="flex-col-1 component row">
      <div class="flex-sm card component row col-12">
        <div class="col-6 intro-text">
          <div class="component-header">
            <h3 class="title title--ad">
              {{ $t("intro.title") }}
            </h3>
          </div>
          <img class="mobile-intro-img" src="@/assets/intro.svg" alt="">
          <div class="component-body">
            <p>
              {{ $t("intro.p1") }}
            </p>
            <p>
              {{ $t("intro.p2") }}
            </p>
          </div>
          <div class="nft-btns">
            <button class="n-button disabled" disabled>🧭 {{ $t("explore") }}</button>
            <button class="n-button disabled" disabled>💡 {{ $t("Create") }}</button>
          </div>
        </div>
        <div class="col-6 intro-img">
          <img src="@/assets/intro.svg" alt="">
        </div>
      </div>
      <div class="flex-sm card component row col-12">
        <div class="col-3 intro2-img">
          <img
            class="image"
            src="@/assets/intro2.svg"
          >
        </div>
        <div class="col-9 text-center flex align-center justify-center intro2-text">
          <div class="banner-get-in-touch-text text-center">
            <h3 class="title title--ad intro-row2" v-html="$t('sec2.title')" />
            <img
              class="mobile-intro-img"
              src="@/assets/intro2.svg"
            >
            <div class="component row tool-usecase">
              <div class="col-3">
                <h4 class="section-heading">
                  {{ $t("sec2.list[0].title") }}
                </h4>
                <div class="section-text">
                  <a href="tel:02 6239 4351">{{ $t("sec2.list[0].desc") }}</a>
                </div>
              </div>
              <div class="col-3">
                <h4 class="section-heading">
                  {{ $t("sec2.list[1].title") }}
                </h4>
                <div class="section-text">
                  <a href="tel:02 6251 1621">{{ $t("sec2.list[1].desc") }}</a>
                </div>
              </div>
              <div class="col-3">
                <h4 class="section-heading">
                  {{ $t("sec2.list[2].title") }}
                </h4>
                <div class="section-text">
                  <a href="tel:0436 455 551">{{ $t("sec2.list[2].desc") }}</a>
                </div>
              </div>
              <div class="col-3">
                <h4 class="section-heading">
                  {{ $t("sec2.list[3].title") }}
                </h4>
                <div class="section-text">
                  <a href="tel:0436 455 551">{{ $t("sec2.list[3].desc") }}</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="less" scoped>
.intro-row2 {
  margin-bottom: 40px;
}
.title {
  text-transform: none;
  line-height: 3.5rem;
}
.component-body {
  margin-top: 50px;
}
.nft-btns {
  margin-top: 50px;
}
.n-button {
  min-width: 150px;
  text-align: center;
  font-size: 1.2rem;
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
  &:not(:first-of-type) {
    margin-left: 20px;
  }
}
.intro-text {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: space-between;
}
.intro-img {
  text-align: right;
  img {
    width: 80%;
  }
}
.mobile-intro-img {
  display: none;
  max-width: 300px;
  height: auto;
  margin-top: 50px;
  width: 100%;
}

@media screen and (max-width: 800px) {
  .n-button {
    min-width: 100px;
  }
  .intro-img, .intro2-img {
    display: none;
  }
  .intro-text, .intro2-text {
    flex: 0 0 100%;
    max-width: 100%;
    width: 100%;
  }
  .mobile-intro-img {
    display: block;
  }
  .tool-usecase {
    flex-direction: column;
    margin-top: 50px;
    .col-3 {
      flex: 0 0 100%;
      max-width: 100%;
      width: 100%;
      margin-bottom: 10px;
      padding-bottom: 10px;
      border-bottom: 2px dashed #231f20;
    }
  }
}
.blue {
  color: #6055a2;
}
</style>

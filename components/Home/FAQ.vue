<template>
  <div id="faq" class="component row">
    <div class="flex-col-1 component row">
      <div
        class="card"
      >
        <div class="component-header">
          <h3 class="title title--ad">
            FAQ
          </h3>
          <!-- <p class="title-description">
            From sea to plate
          </p> -->
        </div>
        <div class="component-body">
          <p>
            {{ $t("faqList[0].q") }}
          </p>
          <p class="dashed-border">
            {{ $t("faqList[0].a") }}
          </p>
          <p>
            {{ $t("faqList[1].q") }}
          </p>
          <p class="dashed-border">
            {{ $t("faqList[1].a") }}
          </p>
          <p>
            {{ $t("faqList[2].q") }}
          </p>
          <p class="dashed-border">
            {{ $t("faqList[2].a") }}
          </p>
          <p>
            {{ $t("faqList[3].q") }}
          </p>
          <p class="dashed-border">
            {{ $t("faqList[3].a") }}
          </p>
          <p>
            {{ $t("faqList[4].q") }}
          </p>
          <p class="dashed-border">
            {{ $t("faqList[4].a") }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="less" scoped>
.dashed-border {
  margin-bottom: 20px;
  padding-bottom: 20px;
  border-bottom: 2px dashed #231f20;
}
</style>

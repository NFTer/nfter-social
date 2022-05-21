<template>
  <div id="roadmap" class="component row">
    <div class="flex-col-1 component row">
      <div
        class="card"
      >
        <div class="component-header">
          <h3 class="title title--ad">
            {{ $t("roadMap") }}
          </h3>
          <!-- <p class="title-description">
            From sea to plate
          </p> -->
        </div>
        <div class="component-body">
          <h2>{{ $t("roadMapList[0].title") }}</h2>
          <p>
            {{ $t("roadMapList[0].desc") }}<br>
            {{ $t("feature") }}
            <ul>
              <li>{{ $t("roadMapList[0].feat[0]") }}</li>
              <li>{{ $t("roadMapList[0].feat[1]") }}</li>
            </ul>
          </p>
          <h2>{{ $t("roadMapList[1].title") }}</h2>
          <p>
            {{ $t("roadMapList[1].desc") }}<br>
            {{ $t("feature") }}
            <ul>
              <li>{{ $t("roadMapList[1].feat[0]") }}</li>
              <li>{{ $t("roadMapList[1].feat[1]") }}</li>
              <li>{{ $t("roadMapList[1].feat[2]") }}</li>
            </ul>
          </p>
          <h2>{{ $t("roadMapList[2].title") }}</h2>
          <p>
            {{ $t("roadMapList[2].desc") }}<br>
            {{ $t("feature") }}
            <ul>
              <li>{{ $t("roadMapList[2].feat[0]") }}</li>
              <li>{{ $t("roadMapList[2].feat[1]") }}</li>
              <li>{{ $t("roadMapList[2].feat[2]") }}</li>
              <li>{{ $t("roadMapList[2].feat[3]") }}</li>
            </ul>
          </p>
          <h2>{{ $t("roadMapList[3].title") }}</h2>
          <p>
            {{ $t("roadMapList[3].desc") }}<br>
            {{ $t("feature") }}
            <ul>
              <li>{{ $t("roadMapList[3].feat[0]") }}</li>
              <li>{{ $t("roadMapList[3].feat[1]") }}</li>
              <li>{{ $t("roadMapList[3].feat[2]") }}</li>
            </ul>
          </p>
          <h2>{{ $t("roadMapList[4].title") }}</h2>
          <p>
            {{ $t("roadMapList[4].desc") }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="less" scoped></style>

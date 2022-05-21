<template>
  <div id="team" class="component row">
    <div class="card">
      <div class="component-header">
        <h3 class="title title--ad">
          {{ $t("team") }}
        </h3>
      </div>
      <div class="component-body">
        <div class="team-item">
          <img src="@/assets/images/team/albert.png" alt="albert" class="team-item-img">
          <p class="team-item-name">@Albert.Zhang</p>
          <p class="team-item-role">ENGINEERING & PM</p>
        </div>
        <div class="team-item">
          <img src="@/assets/images/team/leonliu.png" alt="leon" class="team-item-img">
          <p class="team-item-name">@Leon.Liu</p>
          <p class="team-item-role">PM & COMMUNITY</p>
        </div>
        <div class="team-item">
          <img src="@/assets/images/team/xu.png" alt="xu" class="team-item-img">
          <p class="team-item-name">@Yingjian.Xu</p>
          <p class="team-item-role">UI & UX</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="less" scoped>
.card {
  width: 100%;
}
.title {
  margin-bottom: 2rem;
}
.component-body {
  width: 100%;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  .team-item {
    margin-right: 50px;
    .team-item-img {
      width: 200px;
      border-radius: 20px;
    }
    p {
      padding: 0;
      margin: 0;
    }
  }
}
</style>

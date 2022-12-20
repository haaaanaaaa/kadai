<script setup>

</script>

<template>
  <div id="container">
    <div id="sidebar">
      <div id="sidebar-top">
        <div class="search-box">
            <input type="submit" name="submit" value="" />
            <input
              type="search"
              name="search"
              placeholder="ノート検索（全体）"
              color="#A5A5A5"
            />
          </div>
          <div id="sidebar-top-button">
            <a href="#" class="sidebar-top-button-item">
              <div class="sidebar-top-button-icon"></div>
              <p class="icon-title">通知</p>
            </a>
            <a href="#" class="sidebar-top-button-item">
              <div class="sidebar-top-button-icon"></div>
              <p class="icon-title">お気に入り</p>
            </a>
            <a href="#" class="sidebar-top-button-item">
              <div class="sidebar-top-button-icon"></div>
              <p class="icon-title">タスク管理</p>
            </a>
          </div>
      </div>
      <div id="sidebar-bottom">
        <div class="sidebar-bottom-title">グループ</div>
        <a href="#" class="group-box">
            <div class="group-name">aaa</div>
          </a>
          <div>
          <a href="#" class="group-link">グループ詳細・管理 </a>
        </div>
        <div>
          <a href="#" class="group-link">新着ノート </a>
        </div>
      </div>
    </div>
    <div id="main">
      <div id="main-header"></div>
      <div id="main-body">
        <div id="main-box">
          <div class="main-box-header"></div>
          <div class="main-box-body"></div>
        </div>
      </div>
    </div>
  </div>

</template>

<style scoped>

#container {
  width: 100%;
  height: 100%;
  display: flex;
}
#sidebar {
  width: 220px;
  height: 100%;
  filter: drop-shadow(2px 0px 10px rgba(75, 75, 75, 0.25));
}
#sidebar-top {
  position: relative;
  height: 206px;
  width: 100%;
  background-color: #f1f7ff;
}
#sidebar-bottom {
  position: relative;
  height: 724px;
  width: 100%;
  background-color: #e7f1ff;
}

.search-box {
  position: absolute;
  display: flex;
  width: 196px;
  height: 32px;
  left: 12px;
  top: 72px;
}
input[type="submit"] {
  height: 32px;
  width: 32px;
  background: #0f50ba;
  border: 1px solid #0f50ba;
  border-radius: 3px 0px 0px 3px;
}
input[type="search"] {
  height: 32px;
  width: 166px;
  background-color: #ffffff;
  border: 1px solid #0f50ba;
  font-size: 10px;
  border-radius: 0px 3px 3px 0px;
}

#sidebar-top-button {
  position: absolute;
  display: flex;
  height: 68px;
  width: calc(64px * 3);
  top: 120px;
  left: 14px;
  display: flex;
  align-items: center;
  justify-content: center;

}

.sidebar-top-button-item {
  width: 64px;
  height: 68px;
  display: block;
}
.sidebar-top-button-icon {
  width: 44px;
  height: 44px;
  background-color: #ffffff;
  border-radius: 22px;
  border: 1px solid #bfcfe3;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 auto;

}
.icon-title {
  text-align: center;
  color: #545963;
  font-size: 10px;
  font-weight: 700;
  height: 24px;
  align-items: center;
  display: flex;
  justify-content: center;
}
.sidebar-bottom {
  position: relative;
  height: 724px;
  width: 100%;
  background-color: #e7f1ff;
}
.sidebar-bottom-title {
  position: absolute;
  width: 196px;
  height: 24px;
  top: 10px;
  left: 12px;
  font-weight: 700;
  font-size: 10px;
  vertical-align: middle;
  display: flex;
  align-items: center;
}

.group-box {
  display:inline-block;
  position: absolute;
  left: 12px;
  top: 44px;
  width: 196px;
  height: 40px;
  border: 1px solid #0f50ba;
  border-radius: 3px;
}
.group-name {
  padding-left: 12px;
  display: flex;
  align-items: center;
  position: relative;
  height: 100%;
  font-weight: 700;
  font-size: 14px;
  color: #0f50ba;
  border-radius: 3px;
  background-color: #ffffff;

}
.group-name::after {
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  right: 0px;
  top: 0px;
  width: 30px;
  height: 100%;
  background: #d7e8ff;
  border-radius: 0px 3px 3px 0px;
  content: ">";
}

.group-link {
  top: 94px;
  display:inline-block;
  align-items: center;
  width: 220px;
  height: 30px;
  font-size: 12px;
  font-weight: 400;
  color: #0f50ba;

}


#main {
  width: calc(100% - 220px);
  height: 100%;
}
#main-header {
  width: 100%;
  height: 50px;
  background-color: #f1f7ff;
  border-bottom: 1px solid #bfcfe3;
}
#main-body {
  position: relative;
  height: calc(100% - 50px);
  padding: 27px 16px 32px 32px;
}



</style>

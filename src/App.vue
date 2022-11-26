<template>
  <div class="view">
    <div class="top-view">
      <div class="logo-page">
        <img src="./assets/images/logo_page.jpg" alt="这里是一张logo图片" />
      </div>
      <div class="top-navigation"><TopNavigation /></div>
    </div>
    <div class="body-view">
      <div class="side-navigation"><SideNavigation /></div>
      <div class="protocol-view"></div>
    </div>
  </div>
</template>

<script>
import TopNavigation from './Components/TopNavigation.vue';
import SideNavigation from './Components/SideNavigation.vue';
export default {
  name: 'App',
  components: {
    TopNavigation,
    SideNavigation,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
.view {
  flex-direction: column;
  display: flex;
  height: 850px;
}

.top-view {
  display: flex;
  background-color: #2a3139;
  height: 80px;
}
.body-view {
  flex: 1;
  display: flex;
}

.logo-page img {
  width: 200px;
  height: 80px;
}
.top-navigation {
  flex: 1;
}
.side-navigation {
  width: 200px;
  height: 100%;
  background-color: #2a3139;
}
.protocol-view {
  flex: 1;
}
</style>

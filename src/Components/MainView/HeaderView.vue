<template>
  <div>
    <div class="location">{{ url }}</div>
    <div class="view-title">新增二级商协议</div>
  </div>
</template>
<script>
// 主体的顶部
export default {
  name: 'HeaderView',
  data() {
    return {
      url: window.location.href,
    };
  },
};
</script>
<style scoped>
.location {
  margin: 20px;
  margin-bottom: 10px;
  font-size: 14px;
  color: gray;
}
.view-title {
  margin-left: 20px;
  margin-top: 10px;
  color: black;
  font-size: 22px;
}
</style>

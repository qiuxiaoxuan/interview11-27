<template>
  <div class="dashed">
    <div class="dashed-left"></div>
    <div class="solt-item">
      <slot name="item"></slot>
    </div>
    <div class="dashed-right"></div>
  </div>
</template>
<script>
export default {
  // 协议主体
  name: 'ArticalTitle',
};
</script>
<style scoped>
.dashed {
  display: flex;
  margin-top: 10px;
  padding-top: 10px;
  height: 28px;
}
.solt-item {
  margin-top: -10px;
  width: 100px;
  font-size: 18px;
  font-weight: 700;
  text-align: center;
}
.dashed-left,
.dashed-right {
  flex: 1;
  height: 0;
  border-top: 1px dashed gray;
}
.solt-item img {
  width: 20px;
  margin-right: 6px;
  text-align: center;
}
</style>

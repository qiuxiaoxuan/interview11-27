<template>
  <div>
    <el-menu
      :default-active="activeIndex"
      class="el-menu-demo"
      mode="horizontal"
      @select="handleSelect"
    >
      <el-menu-item index="1">
        <img src="../assets/images/fangzi.png" alt="图标" />
        首页</el-menu-item
      >

      <el-menu-item index="2"
        ><img
          src="../assets/images/fangzi.png"
          alt="图标"
        />主数据</el-menu-item
      >
      <el-menu-item index="3"
        ><img
          src="../assets/images/fangzi.png"
          alt="图标"
        />辖区管理</el-menu-item
      >
      <el-menu-item index="4"
        ><img
          src="../assets/images/fangzi.png"
          alt="图标"
        />销讯通</el-menu-item
      >
    </el-menu>
  </div>
</template>

<script>
export default {
  data() {
    return {
      activeIndex: '1',
    };
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    },
  },
};
</script>
<style scoped>
.el-menu-demo {
  background-color: #2a3139;
  height: 80px;
}
.el-menu.el-menu--horizontal {
  border-bottom: 0 !important;
}
.el-menu-item {
  width: 200px;
  height: 80px !important;
  padding-top: 10px;
  text-align: center;
  color: #fff !important;
}
.el-menu-item img {
  width: 40px;
  margin-right: 8px;
}
</style>

<template>
  <div class="additional">
    <ArticalTitle>
      <div slot="item">
        <img src="../../assets/images/3xuhao.png" alt="" />补充协议
      </div>
    </ArticalTitle>
    <div class="header">
      <div class="protocol">
        <div class="protocol-child1">补充协议1</div>
        <div class="protocol-child">补充协议2</div>
        <div class="protocol-child">补充协议3</div>
      </div>
      <div class="add-button"><button>新增</button></div>
    </div>
    <div class="body-protocol">
      <div class="one">
        <span>协议内容：</span>
        <div class="delete-button"><button>删除</button></div>
      </div>
      <div class="text-area"><textarea></textarea></div>
    </div>
  </div>
</template>
<script>
// 补充协议组件
import ArticalTitle from './ArticalTitle.vue';
export default {
  name: 'AdditionalProtocol',
  components: {
    ArticalTitle,
  },
};
</script>
<style scoped>
.body-protocol {
  margin-top: 10px;
  padding-left: 20px;
  background-color: #fff;
}
.one {
  display: flex;
  padding-top: 25px;
}
.body-protocol span {
  flex: 1;
  font-size: 16px;
  font-weight: 700;
  color: black;
}
.body-protocol .delete-button button {
  margin-right: 10px;
  width: 60px;
  height: 26px;
  text-align: center;
  font-size: 14px;
  line-height: 26px;
  color: #fecc87;
  background-color: #fff;
  border: 1px solid rgba(0, 0, 0, 0.1);
}
.body-protocol .text-area textarea {
  margin-top: 10px;
  margin-bottom: 40px;
  width: 100%;
  height: 150px;
  background-color: #f5f5f5;
  border: 1px solid rgba(0, 0, 0, 0.1);
}
.additional {
  margin-top: 10px;
  padding: 5px 15px;
  background-color: #f5f5f5;
}
.header {
  display: flex;
}
.protocol {
  display: flex;
  flex: 1;
}
.protocol-child,
.protocol-child1 {
  width: 150px;
  height: 36px;
  font-size: 16px;
  color: gray;
  line-height: 36px;
  text-align: center;
  background-color: #fff;
  border: 1px solid rgba(0, 0, 0, 0.1);
}
.protocol-child1 {
  font-weight: 700;
  color: #4f8cff;
}
.add-button button {
  margin-right: 10px;
  width: 80px;
  height: 36px;
  font-size: 16px;
  line-height: 36px;
  color: #fff;
  background-color: #4f8cff;
  border-radius: 4px;
  border: none;
}
</style>

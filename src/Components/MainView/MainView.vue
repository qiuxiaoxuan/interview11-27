<template>
  <div>
    <HeaderView />
    <ProtocolBouncers />
    <ProductPolicy />
    <div><AdditionalProtocol /></div>
    <div class="footer"><button>保存</button></div>
  </div>
</template>
<script>
// 主体视窗组件
// 引入头部
import HeaderView from './HeaderView.vue';
// 引入协议主体组件
import ProtocolBouncers from './ProtocolBouncers.vue';
// 引入产品政策组件
import ProductPolicy from './ProductPolicy.vue';
// 引入补充协议组件
import AdditionalProtocol from './AdditionalProtocol.vue';
export default {
  name: 'MainView',
  components: {
    HeaderView,
    ProtocolBouncers,
    ProductPolicy,
    AdditionalProtocol,
  },
};
</script>
<style scoped>
.footer button {
  margin: 25px 0 15px 20px;
  width: 80px;
  height: 36px;
  font-size: 16px;
  line-height: 36px;
  text-align: center;
  color: #fff;
  background-color: #4f8cff;
  border: none;
  border-radius: 8px;
}
</style>

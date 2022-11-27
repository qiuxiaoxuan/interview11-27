<template>
  <div class="protocal">
    <ArticalTitle>
      <div slot="item">
        <img src="../../assets/images/3xuhao.png" alt="" />协议主体
      </div>
    </ArticalTitle>
    <ProtocolForm />
  </div>
</template>
<script>
// 协议主体
// 引入标题组件
import ArticalTitle from './ArticalTitle.vue';
// 引入协议表单组件
import ProtocolForm from './ProtocolForm.vue';
export default {
  name: 'ProtocolBouncers',
  components: {
    ArticalTitle,
    ProtocolForm,
  },
};
</script>
<style scoped>
.protocal {
  margin-top: 10px;
  padding: 5px 15px;
  background-color: #f5f5f5;
}
</style>

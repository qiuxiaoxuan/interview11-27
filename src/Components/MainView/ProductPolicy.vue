<template>
  <div class="product">
    <ArticalTitle>
      <div slot="item">
        <img src="../../assets/images/3xuhao.png" alt="" />产品政策
      </div>
    </ArticalTitle>
    <div class="header">
      <div class="add-product">
        <span class="blue-box">添加产品</span>
        <span class="text">购进总指标 (万元)：</span>
        <span class="money">￥152.65</span>
      </div>
      <div class="quarter">
        <span class="text">指标按季度分解 (万元)：</span>
        <span class="money">【Q1】￥12.5，</span>
        <span class="money">【Q1】￥12.5，</span>
        <span class="money">【Q1】￥12.5，</span>
        <span class="money">【Q1】￥12.5</span>
      </div>
      <div class="net-all">
        <span class="text">纯销总指标 (万元)：</span>
        <span class="money">￥152.65</span>
      </div>
    </div>
    <div class="product-message">
      <div class="select-product">
        <span class="text">产品：</span>
        <input type="text" placeholder="选择产品" />
        <span class="blue-text">美复胶丸 24粒/盒</span>
      </div>
      <div class="protocol-time">
        <span class="text">协议效期： </span>
        <input type="text" placeholder="2020-02-01 - 2020-05-01" />
      </div>
      <div class="delete-button"><button>删除</button></div>
    </div>
    <form>
      <div class="form-one">
        <div class="title-parent">
          <div class="title-child">协议价 (元)</div>
          <div class="title-child">票折 (元)</div>
          <div class="title-child">购进指标量 (大单位)</div>
          <div class="title-child">购进指标量 (小单位)</div>
          <div class="title-child">购进金额 (万元)</div>
          <div class="title-child">纯销指标量 (小单位)</div>
          <div class="title-child">纯销指标金额 (万元)</div>
        </div>
        <div class="body-parent">
          <div class="body-child">
            <input type="text" placeholder="请输入" />
          </div>
          <div class="body-child">
            <input type="text" placeholder="请输入" />
          </div>
          <div class="body-child">
            <input type="text" placeholder="请输入" />
          </div>
          <div class="body-child">
            <input type="text" placeholder="请输入" />
          </div>
          <div class="body-child">
            <input type="text" placeholder="请输入" />
          </div>
          <div class="body-child">
            <input type="text" placeholder="请输入" />
          </div>
          <div class="body-child">
            <input type="text" placeholder="请输入" />
          </div>
        </div>
      </div>
      <div class="form-two">
        <div class="title-parent">
          <div class="title-child">分销奖励</div>
          <div class="title-child">费用科目</div>
          <div class="title-child">零售配送</div>
          <div class="title-child">费用科目</div>
          <div class="title-child">医疗配送商</div>
          <div class="title-child">费用科目</div>
          <div class="title-child">自定义7</div>
          <div class="title-child">自定义8</div>
        </div>
        <div class="body-parent">
          <div class="body-child">
            <input type="text" placeholder="请输入" />
          </div>
          <div class="body-child">
            <select>
              <option value="1">单选项1</option>
              <option value="2">单选项2</option>
            </select>
          </div>
          <div class="body-child">
            <input type="text" placeholder="请输入" />
          </div>
          <div class="body-child">
            <select>
              <option value="1">单选项1</option>
              <option value="2">单选项2</option>
            </select>
          </div>
          <div class="body-child">
            <input type="text" placeholder="请输入" />
          </div>
          <div class="body-child">
            <select>
              <option value="1">单选项1</option>
              <option value="2">单选项2</option>
            </select>
          </div>
          <div class="body-child">
            <input type="text" placeholder="请输入" />
          </div>
          <div class="body-child">
            <select>
              <option value="1">单选项1</option>
              <option value="2">单选项2</option>
            </select>
          </div>
        </div>
      </div>
    </form>
  </div>
</template>
<script>
// 产品政策组件
import ArticalTitle from './ArticalTitle.vue';
export default {
  name: 'ProductPolicy',
  components: {
    ArticalTitle,
  },
};
</script>
<style scoped>
form {
  flex-direction: column;
  display: flex;
  padding: 20px;
  background: #fff;
}
.title-parent {
  display: flex;
  height: 26px;
  color: gray;
  font-weight: 700;
  line-height: 26px;
  background-color: #f8f8f8;
  border: 1px solid rgba(0, 0, 0, 0.2);
}
.title-child {
  flex: 1;
  padding-left: 10px;
}
.body-parent {
  display: flex;
  padding-top: 11px;
  height: 39px;
  border: 1px solid rgba(0, 0, 0, 0.1);
}
.body-child {
  flex: 1;
  padding-left: 10px;
}
form input {
  padding-left: 10px;
  height: 28px;
  background-color: #f8f8f8;
  border: 1px solid rgba(0, 0, 0, 0.1);
}
form .body-child select {
  padding-left: 10px;
  width: 200px;
  height: 28px;
  border: 1px solid rgba(0, 0, 0, 0.1);
}

.product {
  margin-top: 10px;
  padding: 5px 15px;
  background-color: #f5f5f5;
}
.header {
  display: flex;
  margin-bottom: 10px;
}
.blue-box {
  display: inline-block;
  width: 100px;
  height: 30px;
  font-size: 16px;
  line-height: 30px;
  text-align: center;
  color: #fff;
  background-color: #4f8cff;
  border-radius: 8px;
}
.add-product,
.net-all {
  flex: 1;
}
.quarter {
  flex: 2;
}
.text {
  margin-left: 20px;
  font-size: 14px;
  color: gray;
}
.money {
  font-size: 16px;
  color: gray;
  font-weight: 700;
}

.product-message {
  display: flex;
  margin-bottom: 4px;
  padding: 18px 0 0 30px;
  height: 40px;
  background-color: #fff;
}
.select-product {
  flex: 1;
}
.select-product input {
  width: 90px;
  height: 24px;
  font-size: 16px;
  text-align: center;
  line-height: 24px;
  border: 1px solid rgba(0, 0, 0, 0.1);
}
.protocol-time {
  flex: 2;
}
.protocol-time input {
  width: 250px;
  height: 24px;
  padding-left: 15px;
  font-size: 16px;
  line-height: 24px;
  border: 1px solid rgba(0, 0, 0, 0.1);
}
.blue-text {
  margin-left: 20px;
  font-size: 14px;
  color: #4f8cff;
}
.delete-button button {
  width: 50px;
  height: 24px;
  margin-right: 10px;
  font-size: 16px;
  line-height: 24px;
  color: #fec777;
  background-color: #fff;
  border: 1px solid rgba(0, 0, 0, 0.1);
}
</style>

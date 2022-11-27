<template>
  <div>
    <form>
      <div class="form-top">
        <div class="left">
          <div class="select-user">
            <label for="user">协议用户：</label>
            <input type="text" placeholder="选择用户" id="user" required />
            上海正也医药有限公司
          </div>
          <div class="purchase">
            购进指标：
            <select>
              <option value="1">金额</option>
              <option value="2">质量</option>
              <option value="3">服务</option>
            </select>
            <input type="text" placeholder="输入金额/数量" />
          </div>
          <div class="sale-area">
            <label for="area">销售区域：</label>
            <input type="text" id="area" placeholder="选择区域" />
            <div class="blue-area">
              全国
              <img src="../../assets/images/fork.png" alt="" />
            </div>
          </div>
          <div class="sale-trench">
            购进渠道：
            <select>
              <option value="1">指定渠道</option>
              <option value="2">空运</option>
              <option value="3">海运</option>
            </select>
            <input type="text" placeholder="请选择渠道" />
          </div>
        </div>
        <div class="right">
          <div class="state">
            <label for="state">协议状态：</label>
            <select id="state">
              <option value="1">正常</option>
              <option value="2">不正常</option>
            </select>
          </div>
          <div class="net-sale">
            <label for="net">纯销指标：</label>
            <input type="text" id="net" placeholder="金额" />
            <input type="text" class="input2" placeholder="输入金额/数量" />
          </div>
          <div class="time">
            <label for="time">签订时间：</label>
            <input type="text" id="time" placeholder="2020-02-01  18:25" />
          </div>
        </div>
      </div>
      <div class="footer">
        <div class="footer1">
          <div class="child-flex">指定渠道编码</div>
          <div class="child-flex">指定渠道名称</div>
          <div class="child-flex">所在省</div>
        </div>
        <div class="footer2">
          <div class="child-flex">BJ000090</div>
          <div class="child-flex">宁波九州通药业有限公司</div>
          <div class="child-flex">浙江省</div>
        </div>
        <div class="footer3">
          <div class="child-flex">BJ000192</div>
          <div class="child-flex">国药控股精华有限公司</div>
          <div class="child-flex">浙江省</div>
        </div>
        <div class="footer4">
          <div class="child-flex">BJ000283</div>
          <div class="child-flex">老百姓药业有限公司</div>
          <div class="child-flex">浙江省</div>
        </div>
      </div>
    </form>
  </div>
</template>
<script>
// 协议表单组件
export default {
  name: 'ProtocolForm',
  data() {
    return {
      options: [
        {
          value: '选项1',
          label: '客户1',
        },
      ],
      value: '',
    };
  },
};
</script>
<style scoped>
form {
  padding: 20px;
  background: #fff;
}
.form-top {
  display: flex;
}
.left {
  width: 50%;
}
.right {
  flex: 1;
}
.select-user,
.purchase,
.sale-area,
.state,
.time,
.net-sale {
  margin-bottom: 20px;
}
.select-user input {
  width: 100px;
  height: 20px;
  margin-right: 10px;
  text-align: center;
}
select {
  margin: 0 10px 0 -5px;
  padding-left: 4px;
  width: 104px;
  height: 24px;
}
.purchase input {
  padding-left: 6px;
  height: 20px;
  background-color: #f8f8f8;
  border: 1px solid gray;
}
.sale-area input {
  width: 100px;
  height: 20px;
  margin-right: 10px;
  text-align: center;
}
.sale-area .blue-area {
  display: inline-block;
  width: 80px;
  height: 20px;
  padding: 3px 0 0 8px;
  border: 1px solid #4e8cfd;
  border-radius: 8px;
  font-size: 12px;
  color: #4e8cfd;
}

.sale-area .blue-area img {
  width: 14px;
  margin-left: 30px;
}
.sale-trench input {
  width: 100px;
  height: 20px;
  text-align: center;
}
.net-sale #net {
  width: 80px;
  height: 20px;
  margin-right: 10px;
  padding-left: 5px;
}
.net-sale .input2 {
  padding-left: 6px;
  height: 20px;
  background-color: #f8f8f8;
  border: 1px solid gray;
}
.time input {
  padding-left: 10px;
}
.footer {
  flex-direction: column;
  display: flex;
  margin-top: 20px;
}
.footer1,
.footer2,
.footer3,
.footer4 {
  flex: 1;
  display: flex;
  margin-top: 5px;
  height: 30px;
  font-size: 14px;
  line-height: 30px;
  border-bottom: 1px solid #e5e5e5;
}
.footer1 {
  background-color: #f8f8f8;
}
.child-flex {
  flex: 1;
}
</style>

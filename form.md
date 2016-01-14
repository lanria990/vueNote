## form 表单



#### checkbox 

checkbox中v-model为全部选中的原因是未修改该model的type类型，默认是string。

eg.
```html
	<input type="checkbox" name="type" v-model="account.type" value="alipay" id="type_0"/> <label for="type_0">支付宝</label>
	<input type="checkbox" name="type" v-model="account.type" value="bank" id="type_1" checked /> <label for="type_1">银行卡</label>

```

```javascript
new Vue({
//...
data:function(){
  return {
  account:{
    type:[]
  }
  }
}
})

```

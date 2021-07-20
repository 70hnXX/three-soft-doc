# ht-format-number

el-input 的扩展类型,包含 el-input 的所有属性

### 基础使用

#### jsx 写法

```javascript
<ht-format-number
  v-model={this.formData.settledAmount}
  disabled={this.cantEditMoney}
  max={10}
  min={0}
  precision-type="money"
  on-set={(e) => this.inputValueChange(index, "chargeManHour", e)}
/>
```

### 进阶使用

### Attributes

|      参数      |   说明   |  类型  | 默认值 |                         备注                          |
| :------------: | :------: | :----: | :----: | :---------------------------------------------------: |
| precision-type | 精度类型 | string | money  | money:货币类型，保留两位小数;qty:数量类型，不保留小数 |

### Events

|  事件名   |    说明     |   参数    |  备注  |
| :-------: | :---------: | :-------: | :----: |
| eventName | description | attribute | remark |

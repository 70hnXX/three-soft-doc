### ht-setting-table:

```javascript
<ht-setting-table
    :data="tableData"
    @selectChange="selectChange"
    :enable-table-setting="true"
    :columns="tableColumns"
    pagination
    :total="totalSize"
    :selected-rows.sync="selectedRows"
    :current-page.sync="currentPage"
    @pageChange="_handleSizeChange"
    table-name="kpi"
/>
```

### Attributes

|        参数        |                说明                |   类型   | 默认值 |       备注       |
| :----------------: | :--------------------------------: | :------: | :----: | :--------------: |
|        data        |              表格数据              |  Array   |   -    |        []        |
| selected-rows.sync |             表格选中项             |  Array   |   -    |        -         |
|    selectChange    |         表格选中项发生改变         | Function |   -    |        -         |
|  *selection-type*  | 显示选择框是否多选，需要column配置 |  string  |   ""   | "multiple"为多选 |

### 显示多选按钮

1. 设置：*selection-type*="multiple"

2. column设置

   ```javascript
   {
     prop: "multiple",
     label: "选择",
     type: "multiple",
     width: CELL_WIDTH.multiple,
     cantExport: true
   }
   ```

   


# dbshop
发布商品、选择属性

#### 介绍

* dbshop.js的主要功能就是勾选一个或多个商品属性，生成表格，依赖jQuery;
* 属性可多可少，完全自适应;
* 演示地址：[dbshop.js](http://runjs.cn/detail/kuvsjt0a),也可查看示例，或下载到本地运行;

#### 用法

html:

* 每组属性必须添加class='J_Prorow'和data-index="0"(0是可变的，第一个属性就是0，第二个就是1，以此类推)。

* 勾选input必须添加class="J_Checkbox"和value="sx1:1"("sx1"表示每组属性唯一键名,用于获取JSON的KEY名，"1"表是排序)

* table必须添加id="J_table"
```
<div class="col-md-11 J_Prorow" data-index="0">
	<label class="checkbox-inline">
	  <input type="checkbox" class="J_Checkbox" value="sx1:1">
	  <input type="text" value="军绿色" class="form-control" name="color" disabled="disabled">
	</label>
	<label class="checkbox-inline">
		<input type="checkbox" class="J_Checkbox" value="sx1:2">
		<input type="text" value="黑色" class="form-control" name="color" disabled="disabled">
	</label>
	<label class="checkbox-inline">
	  <input type="checkbox" class="J_Checkbox"  value="sx1:3">
		<input type="text" value="天蓝色" class="form-control" name="color" disabled="disabled">
	</label>
</div>
```

```
<table class="table table-bordered" id="J_table">
	<thead>
		<tr>
			<th>颜色</th>
			<th>尺码</th>
			<th>风格</th>
			<th>魅力</th>
			<th>价格</th>
			<th>数量</th>
			<th>条码</th>
		</tr>
	</thead>
	<tbody></tbody>
</table>
```

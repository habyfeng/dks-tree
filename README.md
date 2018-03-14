# dks-tree
customize of bootstrap-treeview
## 用法
```html
<link rel="stylesheet" type="text/css" href="dks-tree.css" ></link>

<script type="text/javascript" src="jquery-1.11.1.js" ></script>
<script type="text/javascript" src="dks-tree.js" ></script>

<div  id="divTree"></div>
```
```javascript
$("#divTree").dksTree(option);
```
### 数据结构
示例:
```javascript
 var option = {
		data: mpData,
		backColor: "#F6F8FE",
		onhoverColor: "#E4F5FE",
		showBorder: false,
		onNodeSelected: handleNodeSelected
}
```

#### data:JSON对象,属性包括
```javascript
var data = {
		nodeId: id,
		parentId: parentid,
		text: text,
		value: value,
		icon: icon,
		selectedIcon: selectedIcon
}
```
带\*的为必须属性

nodeId*:节点编号,必须为自然数

parentId*:父节点编号

text:节点显示的文本,可选属性

value:存放需要的数据

icon: 节点前的图标的URL

selectedIcon:节点选中时的icon的URL
#### 配置
##### backColor
节点背景颜色,默认值#FFFFFF
##### onhoverColor
鼠标移上时节点的背景颜色
##### showBorder
是否显示节点边框,默认true
#### 事件
onNodeSelected
节点选中事件处理函数

function onNodeSelected(event,data){

}
#### 其它配置
其它配置参考bootstrap-treeview




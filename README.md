# tooltip 使用说明

## 使用 jquery 插件模式编写

## 使用说明

### 引入依赖和插件
```
<link rel="stylesheet" type="text/css" href="path-to/css/tooltip.css">
<script type="text/javascript" src="path-to/js/jquery.js"></script>
<script type="text/javascript" src="path-to/js/tooltip.js"></script>
```

### 初始化

html 代码如下
```
<div class="tool-tip" id="tipTwo">
	<div class="tip-touch" id="touchTwo">
		<div class="tooltip-button">
			提示
		</div>
	</div>
</div>
```
将对应的DOM初始化为 tooltip 插件
```
$("#tipOne").toolTip('init', {
	'text': 'this is test one',
	'width': '360'
});
```

### 绑定 tooltip 显示与隐藏 事件
```
$("#touchOne").click(function() {
	$("#tipOne").toolTip('hideShow')
});
```

## API

- 指定 tooltip 提示内容(text)
	可以是文本，但不限于文本，可以插入 html 字符串, 如 `<div class='my-class'>and so on</div>`

- 指定 tooltip 提示框宽度(width)，宽度不需要加单位，默认使用 px 为单位

## 优势

tooltip 自动检测界面，提示弹层会自动选择从左侧还右侧弹出，以适应界面展示

## 不足

仅仅实现了初步功能，满足了初步需求

# 个人浏览器导航起始网站

项目地址：https://github.com/xcdmrCHP/indexWebSite

## 功能

- **单页面，纯HTML+原生js+原生css，加载速度快**
- 简洁高效
- 夜间模式
- 站内搜索
- 设置链接备注
- 快捷分析
- 分类卡片显示

## 使用

直接下载 `index.html`即可，可本地直接浏览器打开文件访问，也可部署到任何服务器、主机，不需要专门的环境

## 可配置项目

- 主json，网站链接内容

位于 `<body>`标签结束后

```js
web={
	"v":"6",
	"right":{ //导航栏右侧
		"first":[ //右侧上半部分
			{"url":"链接","title":"名称","text":"备注"},
            ...
		],
		"second":[ //右侧下半部分
			{"url":"链接","title":"名称","text":"备注"},
            ...
		]
	},
	"left":{ //导航栏左侧
		"first":[ //左侧上半部分
			{"url":"链接","title":"名称","text":"备注"},
			...
		],
		"second":[ //左侧下半部分
			{"url":"链接","title":"名称","text":"备注"},
			...
		],
		"div":[ //左侧中间的分类折叠卡片
			{
				"name": "分类名称",
				"links":[
			        {"url":"链接","title":"名称","text":"备注"},
                    ...
				]
			},
			...
		],
	},
}
```

- 搜索引擎
- 语录（单击随机显示）

---
menu: "游戏开发"
title: "Shader"
excerpt: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Praesent elementum facilisis leo vel fringilla est ullamcorper eget. At imperdiet dui accumsan sit amet nulla facilities morbi tempus.'
coverImage: '/assets/blog/preview/cover.jpg'
date: '2020-03-16T05:35:07.322Z'
author:
  name: Crying Cat
  picture: '/assets/blog/authors/head.jpg'
ogImage:
  url: '/assets/blog/preview/cover.jpg'
---

# Unity Shader

## Shader Lab

### 文件格式

```
Shader "ShaderName" {
	
}

// Shader关键字 Shader名称 {
// 		shader代码	
// }
```

ShaderName可以是一个路径格式，例如：Test/Shader1，这有点像unity编辑器扩展的MenuItem。

------



### 属性：Properties

```
Shader "ShaderName" {
	Properties {
		PropName1 {"displayName", PropertiesType} = DefaultValue
	}	
}

// Properties关键字 {
// 		变量名 {Inspector显示的变量名称, 变量名称} = 赋值默认值
// }
```

属性相当于Unity中C#脚本的public变量，他能显示在Inspector面板中。

变量不定义在Properties语义块中也可以使用，只是这么做属性将不会显示在Inspector面板中

------



### 数据类型

**_Int**

**_Float**

**_Range**

**_Color**

**_Vector**

**_2D**

**_3D**

**_Cube**

![image-20221203225337865](./assets/image-20221203225337865.png)

------



### 子着色器：SubShader

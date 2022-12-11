---
menu: "游戏开发"
title: "游戏引擎"
excerpt: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Praesent elementum facilisis leo vel fringilla est ullamcorper eget. At imperdiet dui accumsan sit amet nulla facilities morbi tempus."
coverImage: "/assets/blog/preview/cover.jpg"
date: "2020-03-16T05:35:07.322Z"
author:
  name: Crying Cat
  picture: "/assets/blog/authors/head.jpg"
ogImage:
  url: "/assets/blog/preview/cover.jpg"
---

# 引擎分层架构

1.   工具层
2.   功能层
3.   资源层
4.   核心层
5.   平台层

# 地形大气和云的渲染

Height Map高度灰度图

使用分形思想

Lod

视角空间的自适应曲面细分

地形连续不同于单个物体

 对于一个游戏物体，fov越小，绘制所占的像素点越多，效果看起来是放大的



基于矩形的曲面细分

T-Junctions问题

一条边的两侧，细分程度不一样

1.   强制细分少的继续细分到相同程度
2.   面积为0，退化三角形

对于一个等腰三角形，取最长边中点等分成两个等腰三角形的细分方法

QuadTree 四叉树曲面细分



大地图三角形冗余

clip-map lod

mesh lod



hull shader

tessellator

domain shader



amplification shader

mesh shader



marching cubes



Terrain Materials

1.   base color
2.   normal
3.   roughness
4.   height



Texture Array

固定层次，没有中间值，整数层索引得到texture



color mapping

bump mapping

parallax mapping

displacement mapping



virtual texture

浮点数精度溢出导致抖动

相机相对性渲染

相机坐标回归世界坐标





树的渲染

decorator rendering



道路渲染

Spline 样条曲线

Decals （弹坑）



Participating Media

Volume Render Equation



瑞利散射

米散射

# 渲染管线、后期处理

SSAO

HBAO

GTAO

RTAO 



# 图形渲染




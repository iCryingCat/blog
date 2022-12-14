[TOC]



# U2Render

# 开发目标

基于c++语言设计、开发实现一个3D图形渲染引擎。

1.   初级目标：输出目标网格模型
2.   二级目标：输出纹理模型
3.   三级目标：支持动态渲染

------

# 架构设计

## 开发环境

>   vscode：轻量、插件支持
>
>   c++：效率高
>
>   cmake：提供多平台的编译方案

## 支持的3D模型格式

>   FBX

## 图形窗口

>   MFC + D11：window应用窗口，不支持跨平台
>
>   OpenGL：提供绘制窗口，支持跨平台
>
>   QT：GUI界面，目前不需要，游戏引擎一般都是用自己的GUI开发编辑界面

## 数学库

>   ### 向量
>
>   1.   向量运算
>   2.   缩放
>   3.   归一化
>
>   ### 矩阵
>
>   1.   线性变换
>        1.   平移
>        2.   旋转
>        3.   缩放
>   2.   MVP矩阵
>   3.   四元数
>
>   减少依赖，训练代码能力，不使用第三方库

## 渲染流水线

>   顶点着色器
>
>   图元装配
>
>   几何着色器
>
>   光栅化
>
>   片段着色器
>
>   测试混合
>
>   纹理
>
>   变换

# Resolution

## mathlib

### Float

#### 封装类型

1.   Float2
2.   Float3
3.   Float4

#### 提供功能

1.   加法
2.   减法
3.   乘法
4.   除法

### Vector

#### 封装类型

1.   Vector2
2.   Vector3
3.   Vector4

#### 提供功能

1.   加法
2.   减法
3.   乘法
     1.   点乘
     2.   X乘
4.   除法
5.   模长
6.   单位向量
7.   

### Martix

1.   Matrix2x2
2.   Matrix3x3
3.   Matrix4x4

#### 提供功能

1.   加法
2.   减法
3.   乘法
4.   除法

## Render

## FBX模型数据

FBX SDK

OpenGL图形窗口

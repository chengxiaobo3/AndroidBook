## 第1章 Android体系与系统架构 1
* 1．1 Google生态系统 2
* 1．2 Android系统架构 2
  * 1．2．1 Linux 3
  * 1．2．2 Dalvik与ART 3
  * 1．2．3 Framework 3
  * 1．2．4 Standard libraries 4
  * 1．2．5 Application 4
* 1．3 Android App组件架构 4
  * 1．3．1 Android四大组件如何协同工作 5
  * 1．3．2 应用运行上下文对象 5
* 1．4 Android系统源代码目录与系统目录 6
  * 1．4．1 Android系统源代码目录 6
  * 1．4．2 Android系统目录 8
  * 1．4．3 Android App文件目录 11

## 第2章 Android开发工具新接触 13
* 2．1 Android开发IDE介绍 14
  * 2．1．1 Android Studio初体验 14
  * 2．1．2 Android Studio配置 15
* 2．2 Android Studio高级使用技巧 19
  * 2．2．1 更新SDK 20
  * 2．2．2 Android Studio常用界面 21
  * 2．2．3 导入Android Studio工程 23
* 2．3 ADB命令使用技巧 24
  * 2．3．1 ADB基础 24
  * 2．3．2 ADB常用命令 25
  * 2．3．3 ADB命令来源 29
* 2．4 模拟器使用与配置 29

## 第3章 Android控件架构与自定义控件详解 32
* 3．1 Android控件架构 33
* 3．2 View的测量 34
* 3．3 View的绘制 37
* 3．4 ViewGroup的测量 38
* 3．5 ViewGroup的绘制 39
* 3．6 自定义View 39
  * 3．6．1 对现有控件进行拓展 40
  * 3．6．2 创建复合控件 43
  * 3．6．3 重写View来实现全新的控件 51
* 3．7 自定义ViewGroup 54
* 3．8 事件拦截机制分析 59
## 第4章 ListView使用技巧 65
* 4．1 ListView常用优化技巧 66
  * 4．1．1 使用ViewHolder模式提高效率 66
  * 4．1．2 设置项目间分隔线 68
  * 4．1．3 隐藏ListView的滚动条 68
  * 4．1．4 取消ListView的Item点击效果 68
  * 4．1．5 设置ListView需要显示在第几项 69
  * 4．1．6 动态修改ListView 69
  * 4．1．7 遍历ListView中的所有Item 71
  * 4．1．8 处理空ListView 71
  * 4．1．9 ListView滑动监听 72
* 4．2 ListView常用拓展 74
  * 4．2．1 具有弹性的ListView 75
  * 4．2．2 自动显示、隐藏布局的ListView 76
  * 4．2．3 聊天ListView 79
  * 4．2．4 动态改变ListView布局 85

## 第5章 Android Scroll分析 87
* 5．1 滑动效果是如何产生的 88
  * 5．1．1 Android坐标系 88
  * 5．1．2 视图坐标系 88
  * 5．1．3 触控事件――MotionEvent 89
* 5．2 实现滑动的七种方法 91
  * 5．2．1 layout方法 92
  * 5．2．2 offsetLeftAndRight()与offsetTopAndBottom() 93
  * 5．2．3 LayoutParams 93
  * 5．2．4 scrollTo与scrollBy 94
  * 5．2．5 Scroller 96
  * 5．2．6 属性动画 98
  * 5．2．7 ViewDragHelper 98

## 第6章 Android绘图机制与处理技巧 106
* 6．1 屏幕的尺寸信息 107
  * 6．1．1 屏幕参数 107
  * 6．1．2 系统屏幕密度 107
  * 6．1．3 独立像素密度dp 107
  * 6．1．4 单位转换 108
* 6．2 2D绘图基础 110
* 6．3 Android XML绘图 113
  * 6．3．1 Bitmap 113
  * 6．3．2 Shape 113
  * 6．3．3 Layer 115
  * 6．3．4 Selector 116
* 6．4 Android绘图技巧 117
  * 6．4．1 Canvas 117
  * 6．4．2 Layer图层 121
* 6．5 Android图像处理之色彩特效处理 122
  * 6．5．1 色彩矩阵分析 122
  * 6．5．2 Android颜色矩阵――ColorMatrix 128
  * 6．5．3 常用图像颜色矩阵处理效果 131
  * 6．5．4 像素点分析 134
  * 6．5．5 常用图像像素点处理效果 135
* 6．6 Android图像处理之图形特效处理 137
  * 6．6．1 Android变形矩阵――Matrix 137
  * 6．6．2 像素块分析 142
* 6．7 Android图像处理之画笔特效处理 145
  * 6．7．1 PorterDuffXfermode 145
  * 6．7．2 Shader 149
  * 6．7．3 PathEffect 153
* 6．8 View之孪生兄弟――SurfaceView 155
  * 6．8．1 SurfaceView与View的区别 155
  * 6．8．2 SurfaceView的使用 156
  * 6．8．3 SurfaceView实例 159

## 第7章 Android动画机制与使用技巧 162
* 7．1 Android View动画框架 163
  * 7．1．1 透明度动画 163
  * 7．1．2 旋转动画 163
  * 7．1．3 位移动画 164
  * 7．1．4 缩放动画 164
  * 7．1．5 动画集合 164
* 7．2 Android属性动画分析 165
  * 7．2．1 ObjectAnimator 166
  * 7．2．2 PropertyValuesHolder 168
  * 7．2．3 ValueAnimator 168
  * 7．2．4 动画事件的监听 168
  * 7．2．5 AnimatorSet 169
  * 7．2．6 在XML中使用属性动画 170
  * 7．2．7 View的animate方法 170
* 7．3 Android布局动画 171
* 7．4 Interpolators（插值器） 171
* 7．5 自定义动画 172
* 7．6 Android 5．X SVG矢量动画机制 175
  * 7．6．1 ＜path＞标签 175
  * 7．6．2 SVG常用指令 176
  * 7．6．3 SVG编辑器 177
  * 7．6．4 Android中使用SVG 177
  * 7．6．5 SVG动画实例 181
* 7．7 Android动画特效 188
  * 7．7．1 灵动菜单 188
  * 7．7．2 计时器动画 190
  * 7．7．3 下拉展开动画 191

## 第8章 Activity与Activity调用栈分析 195
* 8．1 Activity 196
  * 8．1．1 起源 196
  * 8．1．2 Activity形态 196
  * 8．1．3 生命周期 196
* 8．2 Android任务栈简介 200
* 8．3 AndroidMainifest启动模式 200
  * 8．3．1 standard 201
  * 8．3．2 singleTop 201
  * 8．3．3 singleTask 201
  * 8．3．4 singleInstance 202
* 8．4 Intent Flag启动模式 203
* 8．5 清空任务栈 203
* 8．6 Activity任务栈使用 204

## 第9章 Android系统信息与安全机制 205
* 9．1 Android系统信息获取 206
  * 9．1．1 android．os．Build 206
  * 9．1．2 SystemProperty 207
  * 9．1．3 Android系统信息实例 208
* 9．2 Android Apk应用信息获取之PackageManager 209
  * 9．2．1 PackageManager 210
* 9．3 Android Apk应用信息获取之ActivityManager 215
* 9．4 解析Packages．xml获取系统信息 218
* 9．5 Android安全机制 220
  * 9．5．1 Android安全机制简介 220
  * 9．5．2 Android系统安全隐患 222
  * 9．5．3 Android Apk反编译 223
  * 9．5．4 Android Apk加密 226

## 第10章 Android性能优化 227
* 10．1 布局优化 228
  * 10．1．1 Android UI渲染机制 228
  * 10．1．2 避免Overdraw 229
  * 10．1．3 优化布局层级 229
  * 10．1．4 避免嵌套过多用布局 229
  * 10．1．5 Hierarchy Viewer 234
* 10．2 内存优化 236
  * 10．2．1 什么是内存 236
  * 10．2．2 获取Android系统内存信息 237
  * 10．2．3 内存回收 238
  * 10．2．4 内存优化实例 238
* 10．3 Lint工具 240
* 10．4 使用Android Studio的Memory Monitor工具 240
* 10．5 使用TraceView工具优化App性能 241
  * 10．5．1 生成TraceView日志的两种方法 241
  * 10．5．2 打开TraceView日志 242
  * 10．5．3 分析TraceView日志 242
* 10．6 使用MAT工具分析App内存状态 244
  * 10．6．1 生成HPROF文件 244
  * 10．6．2 分析HPROF文件 245
* 10．7 使用Dumpsys命令分析系统状态 247

## 第11章 搭建云端服务器 248
* 11．1 移动后端服务介绍 249
* 11．2 使用Bmob创建移动后端服务 250
  * 11．2．1 数据服务 251
  * 11．2．2 推送服务 254

## 第12章 Android 5．X新特性详解 257
* 12．1 Android 5．X UI设计初步 258
  * 12．1．1 材料的形态模拟 258
  * 12．1．2 更加真实的动画 258
  * 12．1．3 大色块的使用 259
* 12．2 Material Design主题 260
* 12．3 Palette 261
* 12．4 视图与阴影 263
* 12．5 Tinting和Clipping 265
  * 12．5．1 Tinting（着色） 265
  * 12．5．2 Clipping（裁剪） 267
* 12．6 列表与卡片 269
  * 12．6．1 RecyclerView 269
  * 12．6．2 CardView 275
* 12．7 Activity过渡动画 276
* 12．8 Material Design 动画效果 283
  * 12．8．1 Ripple效果 283
  * 12．8．2 Circular Reveal 285
  * 12．8．3 View state changes Animation 288
* 12．9 Toolbar 293
* 12．10 Notification 296
  * 12．10．1 基本的Notification 297
  * 12．10．2 折叠式Notification 298
  * 12．10．3 悬挂式Notification 300
  * 12．10．4 显示等级的Notification 301

## 第13章 Android实例提高 303
* 13．1 移动迷宫――拼图游戏 304
  * 13．1．1 准备工作 305
  * 13．1．2 初始界面 307
  * 13．1．3 拼图界面 312
  * 13．1．4 效果预览与功能进阶 324
* 13．2 魔幻矩阵――2048 325
  * 13．2．1 2048概述 325
  * 13．2．2 2048游戏分析 326
  * 13．2．3 2048初始化工作 327
  * 13．2．4 小方块设计 328
  * 13．2．5 全局设置 330
  * 13．2．6 游戏面板设计 332
  * 13．2．7 主程序设计 340
  * 13．2．8 功能进阶 341
* 13．3 实战经验总结 342
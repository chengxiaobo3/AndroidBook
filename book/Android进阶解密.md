## 第1章 Android系统架构 1
* 1.1 Android系统架构 1
* 1.2 Android系统源码目录 4
  * 1.2.1 整体结构 4
  * 1.2.2 应用层部分 5
  * 1.2.3 应用框架层部分 6
  * 1.2.4 C/C++程序库部分 6
* 1.3 源码阅读 7
  * 1.3.1 在线阅读 7
  * 1.3.2 使用Source Insight 9
* 1.4 本章小结 12
## 第2章 Android系统启动 13
* 2.1 init进程启动过程 13
  * 2.1.1 引入init进程 13
  * 2.1.2 init进程的入口函数 14
  * 2.1.3 解析init.rc 17
  * 2.1.4 解析Service类型语句 19
  * 2.1.5 init启动Zygote 20
  * 2.1.6 属性服务 23
  * 2.1.7 init进程启动总结 27
* 2.2 Zygote进程启动过程 27
  * 2.2.1 Zygote概述 28
  * 2.2.2 Zygote启动脚本 28
  * 2.2.3 Zygote进程启动过程介绍 30
  * 2.2.4 Zygote进程启动总结 38
* 2.3 SystemServer处理过程 39
  * 2.3.1 Zygote处理SystemServer进程 39
  * 2.3.2 解析SystemServer进程 44
  * 2.3.3 SystemServer进程总结 48
* 2.4 Launcher启动过程 48
  * 2.4.1 Launcher概述 48
  * 2.4.2 Launcher启动过程介绍 49
  * 2.4.3 Launcher中应用图标显示过程 54
* 2.5 Android系统启动流程 59
* 2.6 本章小结 60
## 第3章 应用程序进程启动过程 61
* 3.1 应用程序进程简介 61
* 3.2 应用程序进程启动过程介绍 62
  * 3.2.1 AMS发送启动应用程序进程请求 62
  * 3.2.2 Zygote接收请求并创建应用程序进程 68
* 3.3 Binder线程池启动过程 75
* 3.4 消息循环创建过程 78
* 3.5 本章小结 80
## 第4章 四大组件的工作过程 81
* 4.1 根Activity的启动过程 82
  * 4.1.1 Launcher请求AMS过程 82
  * 4.1.2 AMS到ApplicationThread的调用过程 85
  * 4.1.3 ActivityThread启动Activity的过程 94
  * 4.1.4 根Activity启动过程中涉及的进程 99
* 4.2 Service的启动过程 101
  * 4.2.1 ContextImpl到AMS的调用过程 101
  * 4.2.2 ActivityThread启动Service 103
* 4.3 Service的绑定过程 110
  * 4.3.1 ContextImpl到AMS的调用过程 111
  * 4.3.2 Service的绑定过程 112
* 4.4 广播的注册、发送和接收过程 122
  * 4.4.1 广播的注册过程 122
  * 4.4.2 广播的发送和接收过程 127
* 4.5 Content Provider的启动过程 137
  * 4.5.1 query方法到AMS的调用过程 137
  * 4.5.2 AMS启动Content Provider的过程 143
* 4.6 本章小结 148
## 第5章 理解上下文Context 149
* 5.1 Context的关联类 149
* 5.2 Application Context的创建过程 151
* 5.3 Application Context的获取过程 156
* 5.4 Activity的Context创建过程 156
* 5.5 Service的Context创建过程 161
* 5.6 本章小结 163
## 第6章 理解ActivityManagerService 164
* 6.1 AMS家族 164
  * 6.1.1 Android 7.0的AMS家族 164
  * 6.1.2 Android 8.0的AMS家族 170
* 6.2 AMS的启动过程 171
* 6.3 AMS与应用程序进程 174
* 6.4 AMS重要的数据结构 176
  * 6.4.1 解析ActivityRecord 177
  * 6.4.2 解析TaskRecord 177
  * 6.4.3 解析ActivityStack 178
* 6.5 Activity栈管理 181
  * 6.5.1 Activity任务栈模型 181
  * 6.5.2 Launch Mode 182
  * 6.5.3 Intent的FLAG 182
  * 6.5.4 taskAffinity 185
* 6.6 本章小结 186
## 第7章 理解WindowManager 187
* 7.1 Window、WindowManager和WMS 187
* 7.2 WindowManager的关联类 188
* 7.3 Window的属性 193
  * 7.3.1 Window的类型和显示次序 193
  * 7.3.2 Window的标志 195
  * 7.3.3 软键盘相关模式 196
* 7.4 Window的操作 196
  * 7.4.1 系统窗口的添加过程 197
  * 7.4.2 Activity的添加过程 202
  * 7.4.3 Window的更新过程 203
* 7.5 本章小结 206
## 第8章 理解WindowManagerService 207
* 8.1 WMS的职责 207
* 8.2 WMS的创建过程 209
* 8.3 WMS的重要成员 217
* 8.4 Window的添加过程（WMS处理部分） 219
* 8.5 Window的删除过程 225
* 8.6 本章小结 230
## 第9章 JNI原理 231
* 9.1 系统源码中的JNI 232
* 9.2 MediaRecorder框架中的JNI 233
  * 9.2.1 Java Framework层的MediaRecorder 233
  * 9.2.2 JNI层的MediaRecorder 234
  * 9.2.3 Native方法注册 235
* 9.3 数据类型的转换 239
  * 9.3.1 基本数据类型的转换 240
  * 9.3.2 引用数据类型的转换 240
* 9.4 方法签名 242
* 9.5 解析JNIEnv 244
  * 9.5.1 jfieldID和jmethodID 245
  * 9.5.2 使用jfieldID和jmethodID 247
* 9.6 引用类型 249
  * 9.6.1 本地引用 249
  * 9.6.2 全局引用 249
  * 9.6.3 弱全局引用 250
* 9.7 本章小结 251
## 第10章 Java虚拟机 252
* 10.1 概述 252
  * 10.1.1 Java虚拟机家族 253
  * 10.1.2 Java虚拟机执行流程 253
* 10.2 Java虚拟机结构 254
  * 10.2.1 Class文件格式 255
  * 10.2.2 类的生命周期 256
  * 10.2.3 类加载子系统 257
  * 10.2.4 运行时数据区域 258
* 10.3 对象的创建 260
* 10.4 对象的堆内存布局 262
* 10.5 oop-klass模型 263
* 10.6 垃圾标记算法 266
  * 10.6.1 Java中的引用 266
  * 10.6.2 引用计数算法 267
  * 10.6.3 根搜索算法 269
* 10.7 Java对象在虚拟机中的生命周期 270
* 10.8 垃圾收集算法 271
  * 10.8.1 标记—清除算法 271
  * 10.8.2 复制算法 272
  * 10.8.3 标记—压缩算法 273
  * 10.8.4 分代收集算法 274
* 10.9 本章小结 275
## 第11章 Dalvik和ART 276
* 11.1 Dalvik虚拟机 276
  * 11.1.1 DVM与JVM的区别 276
  * 11.1.2 DVM架构 278
  * 11.1.3 DVM的运行时堆 280
  * 11.1.4 DVM的GC日志 280
* 11.2 ART虚拟机 281
  * 11.2.1 ART与DVM的区别 281
  * 11.2.2 ART的运行时堆 282
  * 11.2.3 ART的GC日志 283
* 11.3 DVM和ART的诞生 285
* 11.4 本章小结 288
## 第12章 理解ClassLoader 289
* 12.1 Java中的ClassLoader 289
  * 12.1.1 ClassLoader的类型 289
  * 12.1.2 ClassLoader的继承关系 291
  * 12.1.3 双亲委托模式 292
  * 12.1.4 自定义ClassLoader 295
* 12.2 Android中的ClassLoader 298
  * 12.2.1 ClassLoader的类型 298
  * 12.2.2 ClassLoader的继承关系 300
  * 12.2.3 ClassLoader的加载过程 302
  * 12.2.4 BootClassLoader的创建 306
  * 12.2.5 PathClassLoader的创建 309
* 12.3 本章小结 311
## 第13章 热修复原理 312
* 13.1 热修复的产生 312
* 13.2 热修复框架的种类和对比 313
* 13.3 资源修复 314
  * 13.3.1 Instant Run概述 314
  * 13.3.2 Instant Run的资源修复 315
* 13.4 代码修复 318
  * 13.4.1 类加载方案 319
  * 13.4.2 底层替换方案 321
  * 13.4.3 Instant Run方案 322
* 13.5 动态链接库的修复 323
  * 13.5.1 System的load和loadLibarary方法 323
  * 13.5.2 nativeLoad方法分析 327
* 13.6 本章小结 333
## 第14章 Hook技术 334
* 14.1 Hook技术概述 334
* 14.2 Hook技术分类 336
* 14.3 代理模式 336
  * 14.3.1 代理模式简单实现 337
  * 14.3.2 动态代理的简单实现 338
* 14.4 Hook startActivity方法 339
  * 14.4.1 Hook Activity的startActivity方法 340
  * 14.4.2 Hook Context的startActivity方法 343
  * 14.4.3 Hook startActivity总结 344
* 14.5 本章小结 345
## 第15章 插件化原理 346
* 15.1 动态加载技术 346
* 15.2 插件化的产生 347
  * 15.2.1 应用开发的痛点和瓶颈 347
  * 15.2.2 插件化思想 348
  * 15.2.3 插件化定义 350
* 15.3 插件化框架对比 351
* 15.4 Activity插件化 352
  * 15.4.1 Activity的启动过程回顾 352
  * 15.4.2 Hook IActivityManager方案实现 354
  * 15.4.3 Hook Instrumentation方案实现 364
  * 15.4.4 总结 367
* 15.5 Service插件化 368
  * 15.5.1 插件化方面Service与Activity的不同 368
  * 15.5.2 代理分发实现 370
* 15.6 ContentProvider插件化 376
  * 15.6.1 ContentProvider的启动过程回顾 376
  * 15.6.2 VirtualApk的实现 377
* 15.7 BroadcastReceiver的插件化 385
  * 15.7.1 广播插件化思路 386
  * 15.7.2 VirtualApk的实现 386
* 15.8 资源的插件化 387
  * 15.8.1 系统资源加载 387
  * 15.8.2 VirtualApk实现 389
* 15.9 so的插件化 390
* 15.10 本章小结 393
## 第16章 绘制优化 394
* 16.1 绘制性能分析 394
  * 16.1.1 绘制原理 395
  * 16.1.2 Profile GPU Rendering 396
  * 16.1.3 Systrace 398
  * 16.1.4 Traceview 404
* 16.2 布局优化 407
  * 16.2.1 布局优化工具 407
  * 16.2.2 布局优化方法 411
  * 16.2.3 避免GPU过度绘制 419
* 16.3 本章小结 420
## 第17章 内存优化 421
* 17.1 避免可控的内存泄漏 421
  * 17.1.1 什么是内存泄漏 421
  * 17.1.2 内存泄漏的场景 422
* 17.2 Memory Monitor 428
  * 17.2.1 使用Memory Monitor 429
  * 17.2.2 大内存申请与GC 430
  * 17.2.3 内存抖动 430
* 17.3 Allocation Tracker 430
  * 17.3.1 使用Allocation Tracker 431
  * 17.3.2 alloc文件分析 431
* 17.4 Heap Dump 434
  * 17.4.1 使用Heap Dump 434
  * 17.4.2 检测内存泄漏 436
* 17.5 内存分析工具MAT 438
  * 17.5.1 生成hprof文件 438
  * 17.5.2 MAT分析hprof文件 440
* 17.6 LeakCanary 448
  * 17.6.1 使用LeakCanary 449
  * 17.6.2 LeakCanary应用举例 449
* 17.7 本章小结 453
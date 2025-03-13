# Android 性能优化工具

这个目录包含了Android性能优化相关的各类工具介绍、使用教程和示例。

## 内存分析工具

### LeakCanary

[LeakCanary](https://github.com/square/leakcanary) 是Square开源的内存泄漏检测工具，可以在开发阶段自动检测Activity和Fragment的内存泄漏。

**接入指南**：
```gradle
// 在build.gradle中添加
dependencies {
  debugImplementation 'com.squareup.leakcanary:leakcanary-android:2.10'
}
```

使用LeakCanary无需额外代码，它会自动检测并通知开发者内存泄漏问题。

### MAT (Memory Analyzer Tool)

Eclipse提供的内存分析工具，可以分析Android应用的hprof文件，找出内存泄漏和占用过高的对象。

**使用步骤**：
1. 通过Android Studio导出hprof文件
2. 使用Android SDK中的hprof-conv工具转换文件格式
3. 使用MAT打开并分析

## 卡顿分析工具

### AndroidGodEye

[AndroidGodEye](https://github.com/Kyson/AndroidGodEye) 是一个全面的性能监控工具，提供了卡顿、内存、CPU、网络等多维度监控功能。

**接入指南**：
```gradle
dependencies {
  implementation 'cn.hikyson.godeye:godeye-core:VERSION_NAME'
  implementation 'cn.hikyson.godeye:godeye-toolbox:VERSION_NAME'
  debugImplementation 'cn.hikyson.godeye:godeye-monitor:VERSION_NAME'
}
```

### Systrace

Google官方提供的系统级性能分析工具，可以帮助开发者分析应用卡顿问题。

**使用步骤**：
1. 连接设备
2. 执行命令：`python $ANDROID_HOME/platform-tools/systrace/systrace.py --time=10 -o trace.html sched gfx view wm`
3. 打开生成的trace.html文件进行分析

## UI性能分析工具

### Layout Inspector

Android Studio内置的布局检查工具，可以检查布局层级和过度绘制。

### GPU渲染分析

在开发者选项中开启"GPU渲染模式分析"，可以直观地观察每一帧的渲染时间。

## 启动分析工具

### App Startup Library

Google官方提供的应用启动优化库，可以优化多个组件的初始化过程。

**接入指南**：
```gradle
dependencies {
  implementation "androidx.startup:startup-runtime:1.1.1"
}
```

## 网络分析工具

### Charles

强大的HTTP代理工具，可以捕获和分析应用的网络请求。

### Stetho

Facebook开源的Android调试桥，可以通过Chrome开发者工具查看应用的网络请求、数据库内容等。

**接入指南**：
```gradle
dependencies {
  implementation 'com.facebook.stetho:stetho:1.6.0'
  implementation 'com.facebook.stetho:stetho-okhttp3:1.6.0'
}
```

## 全面APM解决方案

### Matrix (腾讯)

腾讯开源的应用性能监控框架，提供了包括内存泄漏、卡顿、IO、网络等多维度的监控能力。

[Matrix GitHub 仓库](https://github.com/Tencent/matrix)

### Booster (字节跳动)

字节跳动开源的性能优化框架，提供了包括包体积优化、图片优化、内存优化等多种能力。

[Booster GitHub 仓库](https://github.com/didi/booster)

## 性能分析最佳实践

1. 在开发阶段使用LeakCanary检测内存泄漏
2. 使用Systrace分析卡顿问题
3. 使用Layout Inspector检查布局层级
4. 使用Charles/Stetho分析网络请求
5. 针对不同性能问题选择适合的工具进行分析

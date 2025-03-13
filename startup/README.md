# Android 启动优化

这个目录包含了Android应用启动性能优化相关的资料、工具和示例代码。

## 主要内容

### 启动类型

- 冷启动 (Cold Start)
- 温启动 (Warm Start)
- 热启动 (Hot Start)
- 各类启动的优化策略

### Application优化

- 懒加载和延迟初始化
- 启动器(如Alpha)实现示例
- 异步初始化非核心组件
- 使用ContentProvider进行初始化

### 白屏优化

- 启动主题(SplashTheme)实现
- 预览窗口(Preview Window)技术
- 启动页设计最佳实践

### 首页优化

- 骨架屏(Skeleton Screen)实现
- 首屏数据加载优化
- 视图加载优化

## 测量与分析

- 使用Firebase Performance监控启动时间
- 自定义启动时间埋点方案
- 分析启动过程的方法跟踪

## 工具

1. [App Startup](https://developer.android.com/topic/libraries/app-startup)
2. [Android Vitals](https://developer.android.com/topic/performance/vitals)
3. [Android Performance Profiler](https://developer.android.com/studio/profile/android-profiler)

## 学习资源

- [Google官方启动优化指南](https://developer.android.com/topic/performance/vitals/launch-time)
- [Android App Cold Start](https://www.youtube.com/watch?v=4-7RxlWVvRI)

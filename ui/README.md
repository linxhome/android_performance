# Android UI渲染优化

这个目录包含了Android UI渲染优化相关的资料、工具和示例代码。

## 主要内容

### 布局优化

- ConstraintLayout使用技巧
- 避免布局嵌套过深
- 使用Systrace分析布局性能
- 自定义View性能优化

### 减少过度绘制

- 使用Layout Inspector检测过度绘制
- 优化背景绘制
- 使用ClipRect避免无用区域的绘制

### 列表滚动优化

- RecyclerView性能优化
- 高效ViewHolder实现
- 图片加载和缓存策略
- 预加载和分页技术

### 动画性能优化

- 使用硬件加速
- 属性动画vs视图动画
- 避免在动画过程中执行复杂操作

## 工具

1. [Systrace](https://developer.android.com/topic/performance/tracing)
2. [Layout Inspector](https://developer.android.com/studio/debug/layout-inspector)
3. [GPU Profiling](https://developer.android.com/topic/performance/rendering/profile-gpu)

## 学习资源

- [Android渲染优化官方文档](https://developer.android.com/topic/performance/rendering)
- [Android Performance Patterns](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc9CBxr3BVjPTPoDPLdPIFCE)

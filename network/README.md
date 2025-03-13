# Android 网络优化

这个目录包含了Android网络性能优化相关的资料、工具和示例代码。

## 主要内容

### 请求优化

- API请求合并和批量处理
- HTTP/2和QUIC协议应用
- gRPC和Protocol Buffers使用
- 请求压缩和优化
- 请求优先级处理

### 缓存策略

- HTTP缓存实现
- 本地数据库缓存设计
- 内存缓存和磁盘缓存结合
- 缓存有效期管理

### 弱网优化

- 请求重试和超时策略
- 断点续传实现
- 弱网环境下的降级策略
- 网络状态感知的请求调度

### 图片加载优化

- 图片尺寸和质量动态调整
- 渐进式图片加载
- WebP格式的应用
- 图片懒加载实现

## 工具和库

1. [OkHttp](https://github.com/square/okhttp)
2. [Retrofit](https://github.com/square/retrofit)
3. [Charles](https://www.charlesproxy.com/)
4. [Android Network Profiler](https://developer.android.com/studio/profile/network-profiler)
5. [Stetho](https://github.com/facebook/stetho)

## 网络性能指标

- 首包时间 (TTFB - Time to First Byte)
- DNS解析时间
- TCP连接时间
- SSL握手时间
- 请求完成时间
- 流量消耗

## 测量与监控

- 网络性能埋点方案
- 使用自定义Interceptor监控网络性能
- 线上数据采集与分析

## 学习资源

- [高性能移动网络](https://developer.android.com/topic/performance/network-xfer)
- [HTTP缓存机制](https://developer.mozilla.org/en-US/docs/Web/HTTP/Caching)

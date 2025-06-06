# ⚙️ 客户端配置优化

## 基础配置

### 🎮 游戏设置优化
```
视频设置推荐配置:
- 图形质量: 流畅 (性能优先) / 精美 (质量优先)
- 渲染距离: 12区块 (推荐) / 8区块 (低配置)
- 平滑光照: 关闭 (提升性能) / 开启 (更好画质)
- 最大帧率: 60 FPS (平衡) / 无限制 (高刷新率显示器)
- 垂直同步: 关闭 (减少输入延迟)
- GUI缩放: 自动 / 根据需要调整
```

### 🔊 音频设置
```
推荐音频配置:
- 主音量: 70%
- 音乐: 50%
- 唱片机/音符盒: 100%
- 天气: 20% (减少雷雨干扰)
- 方块: 100%
- 敌对生物: 100% (重要安全提示)
- 友好生物: 80%
- 玩家: 100%
- 环境: 60%
```

### ⌨️ 控制设置
| 功能 | 推荐按键 | 说明 |
|------|----------|------|
| 攻击/破坏 | 鼠标左键 | 默认 |
| 使用物品/放置方块 | 鼠标右键 | 默认 |
| 背包 | E | 默认 |
| 丢弃 | Q | 默认 |
| 聊天 | T | 默认 |
| 命令 | / | 默认 |
| 截图 | F2 | 默认 |
| 调试屏幕 | F3 | 重要诊断工具 |

## 高级配置

### 🖥️ 启动参数优化
```bash
# 内存配置 (根据你的系统内存调整)
-Xms2G -Xmx4G

# 垃圾回收优化
-XX:+UseG1GC
-XX:+ParallelRefProcEnabled
-XX:MaxGCPauseMillis=200
-XX:+UnlockExperimentalVMOptions
-XX:+DisableExplicitGC
-XX:+AlwaysPreTouch
-XX:G1NewSizePercent=30
-XX:G1MaxNewSizePercent=40
-XX:G1HeapRegionSize=8M
-XX:G1ReservePercent=20
-XX:G1HeapWastePercent=5
-XX:G1MixedGCCountTarget=4
-XX:InitiatingHeapOccupancyPercent=15
-XX:G1MixedGCLiveThresholdPercent=90
-XX:G1RSetUpdatingPauseTimePercent=5
-XX:SurvivorRatio=32
-XX:+PerfDisableSharedMem
-XX:MaxTenuringThreshold=1

# 额外优化
-Dusing.aikars.flags=https://mcflags.emc.gs
-Daikars.new.flags=true
```

### 🎯 性能等级配置

#### 🏃 高性能配置 (适合竞技/PVP)
```
渲染距离: 6-8区块
图形质量: 流畅
平滑光照: 关闭
粒子: 最少
实体阴影: 关闭
实体距离: 50%
云: 关闭
```

#### ⚖️ 平衡配置 (日常游戏)
```
渲染距离: 10-12区块
图形质量: 普通
平滑光照: 最少
粒子: 减少
实体阴影: 关闭
实体距离: 100%
云: 快速
```

#### 🎨 画质配置 (建筑/截图)
```
渲染距离: 16-32区块
图形质量: 精美
平滑光照: 最大
粒子: 全部
实体阴影: 开启
实体距离: 100%
云: 精美
```

## 专用服务器配置

### 🌐 连接优化
```
服务器地址配置:
- 直接IP连接 (最快)
- 使用游戏内置DNS
- 检查防火墙设置
- 关闭不必要的后台程序
```

### 📊 网络优化
| 设置项 | 推荐值 | 说明 |
|--------|--------|------|
| 网络连接 | 有线连接 | 比Wi-Fi更稳定 |
| MTU大小 | 1500 | 默认值通常最佳 |
| TCP缓冲区 | 系统默认 | 避免手动修改 |

## 模组配置

### 🔍 OptiFine配置
```
性能设置:
- 平滑帧率: 开启
- 动态更新: 开启
- 快速渲染: 开启
- 智能动画: 开启
- 平滑世界: 关闭 (可能影响性能)

视觉设置:
- 连接纹理: 精美 (高配置) / 快速 (低配置)
- 随机实体: 开启
- 自定义天空: 开启
- 动态光源: 开启 (消耗性能)
```

### 🗺️ JourneyMap配置
```
性能设置:
- 地图绘制延迟: 2000ms
- 缓存清理间隔: 300秒
- 实时绘制: 关闭 (节省CPU)

显示设置:
- 小地图: 圆形
- 位置: 右上角
- 比例: 2x
- 显示网格: 开启
```

## 资源包配置

### 📦 推荐资源包类型
1. **原版风格改进**
   - Faithful (高清原版风格)
   - Enhanced Default (增强默认)

2. **现代风格**
   - Modern HD
   - Compliance

3. **性能友好**
   - Optifine默认改进
   - 低分辨率包

### 🎨 资源包优化设置
```
加载顺序:
1. 性能优化包 (底层)
2. 纹理改进包 (中层)  
3. 界面美化包 (顶层)

注意事项:
- 避免加载过多资源包
- 定期清理未使用的包
- 监控内存使用情况
```

## 故障排除

### 🐛 常见配置问题
1. **游戏卡顿**
   - 降低渲染距离
   - 关闭不必要的特效
   - 检查内存分配

2. **网络延迟高**
   - 检查网络连接
   - 关闭后台下载
   - 使用有线连接

3. **画面问题**
   - 更新显卡驱动
   - 重置视频设置
   - 检查资源包兼容性

### 📝 配置文件备份
```
重要配置文件位置:
- options.txt (游戏设置)
- servers.dat (服务器列表)
- optionsof.txt (OptiFine设置)
- config/ (模组配置文件夹)

备份建议:
- 定期备份整个 .minecraft 文件夹
- 记录重要的启动参数
- 保存自定义按键配置
```

## 性能监控

### 📊 性能指标
```
监控指标:
- FPS (帧率): F3界面左上角
- 内存使用: F3界面右侧
- 网络延迟: Tab键玩家列表
- TPS (服务器): 部分模组提供

目标数值:
- FPS: >30 (最低) / >60 (理想)
- 内存: <80% 分配内存
- 延迟: <50ms (优秀) / <100ms (可接受)
```

### 🔧 性能调优步骤
1. **基线测试** - 记录当前性能
2. **逐项调整** - 一次只改一个设置
3. **测试验证** - 确认改进效果
4. **记录配置** - 保存最佳设置

---
*好的配置是游戏体验的基础，请根据自己的硬件情况适当调整* 
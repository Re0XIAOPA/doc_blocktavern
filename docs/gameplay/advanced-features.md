# ⚡ 高级功能指南

## 经济系统

### 💰 货币系统
- **基础货币**: 金币 (Gold Coins)
- **获取方式**: 
  - 完成任务奖励
  - 出售物品给商店
  - 与其他玩家交易
  - 参与活动获得

### 🏪 商店系统
```
商店类型:
- 系统商店: 基础物品买卖
- 玩家商店: 自由定价交易
- 拍卖行: 竞价拍卖物品
- 特殊商店: 限时稀有物品
```

### 💳 银行系统
| 功能 | 命令 | 说明 |
|------|------|------|
| 查看余额 | `/balance` | 显示当前金币数量 |
| 转账 | `/pay [玩家] [金额]` | 转账给其他玩家 |
| 银行存款 | `/bank deposit [金额]` | 存入银行获得利息 |
| 银行取款 | `/bank withdraw [金额]` | 从银行取出金币 |

## 领地系统

### 🏰 创建和管理领地
```
基础命令:
/res create [领地名] - 创建领地
/res remove [领地名] - 删除领地
/res info [领地名] - 查看领地信息
/res list - 查看自己的领地列表
```

### 👥 权限管理
```
权限设置:
/res pset [玩家名] [权限] [true/false]

常用权限:
- build: 建造权限
- destroy: 破坏权限
- use: 使用权限
- container: 容器权限
```

### 🔧 高级设置
| 标志 | 功能 | 用法 |
|------|------|------|
| pvp | PVP控制 | `/res set pvp false` |
| monster | 怪物生成 | `/res set monster false` |
| animals | 动物生成 | `/res set animals true` |
| fire | 火焰蔓延 | `/res set fire false` |

## 传送系统

### 🚪 传送点 (Warp)
```
管理传送点:
/warp [传送点名] - 传送到指定地点
/warp list - 查看可用传送点
/setwarp [名称] - 创建传送点 (需要权限)
/delwarp [名称] - 删除传送点 (需要权限)
```

### 🏠 家园系统 (Home)
```
家园管理:
/home - 回到默认家园
/home [家园名] - 传送到指定家园
/sethome [家园名] - 设置家园点
/delhome [家园名] - 删除家园点
/homes - 查看所有家园点
```

### 🎯 传送请求 (TPA)
```
传送请求系统:
/tpa [玩家名] - 请求传送到玩家身边
/tpahere [玩家名] - 请求玩家传送到你身边
/tpaccept - 接受传送请求
/tpdeny - 拒绝传送请求
```

## 任务系统

### 📋 每日任务
- **刷新时间**: 每日北京时间00:00
- **任务类型**: 
  - 采集任务 (挖掘、砍伐、收获)
  - 建造任务 (放置方块、建筑)
  - 探索任务 (访问生物群系、发现结构)
  - 社交任务 (与玩家互动、加入活动)

### 🏆 成就系统
```
成就类别:
- 探索成就: 发现新地区、生物群系
- 建造成就: 建造特定结构、使用材料
- 战斗成就: 击败生物、PVP胜利
- 社交成就: 与玩家互动、加入公会
- 收集成就: 收集稀有物品、完成收藏
```

### 🎁 奖励系统
| 奖励类型 | 获取方式 | 奖励内容 |
|----------|----------|----------|
| 签到奖励 | 每日签到 | 金币、物品、经验 |
| 任务奖励 | 完成任务 | 金币、特殊物品 |
| 成就奖励 | 解锁成就 | 称号、装饰品 |
| 活动奖励 | 参与活动 | 限定物品、装备 |

## 公会系统

### 🤝 创建和加入公会
```
公会管理:
/guild create [公会名] - 创建公会
/guild join [公会名] - 申请加入公会
/guild leave - 离开当前公会
/guild info - 查看公会信息
```

### 👑 公会管理
```
管理权限:
/guild invite [玩家名] - 邀请玩家
/guild kick [玩家名] - 踢出玩家
/guild promote [玩家名] - 提升职位
/guild demote [玩家名] - 降低职位
```

### 🏛️ 公会功能
- **公会仓库**: 共享物品存储
- **公会领地**: 专属建造区域
- **公会聊天**: 内部沟通频道
- **公会活动**: 组织团队活动

## PVP系统

### ⚔️ 战斗机制
```
PVP规则:
- 特定区域开启PVP
- 死亡掉落部分物品
- 击杀获得荣誉点数
- 连续击杀获得连击奖励
```

### 🏟️ 竞技场
- **排位赛**: 定期排名比赛
- **团队战**: 公会间对抗
- **擂台赛**: 1v1单挑模式
- **混战**: 多人自由战斗

### 🎖️ 荣誉系统
| 等级 | 所需荣誉 | 奖励 |
|------|----------|------|
| 新手战士 | 0-100 | 基础PVP装备 |
| 熟练战士 | 101-500 | 进阶武器 |
| 精英战士 | 501-1000 | 特殊护甲 |
| 传奇战士 | 1001+ | 独特称号、装饰 |

## 活动系统

### 🎉 定期活动
```
活动类型:
- 建造比赛: 主题建筑创作
- 寻宝活动: 隐藏物品搜寻
- 团队任务: 合作完成挑战
- 节日庆典: 特殊节日活动
```

### 🏅 活动奖励
- **参与奖**: 所有参与者获得
- **排名奖**: 根据成绩发放
- **特殊奖**: 创意、团队合作等
- **纪念品**: 限定收藏物品

## 插件功能

### 🔌 实用插件
- **ChestShop**: 自动贩售系统
- **LWC**: 容器保护锁定
- **McMMO**: 技能升级系统
- **Jobs**: 职业与工作系统

### 🛠️ 管理插件
- **WorldGuard**: 区域保护
- **EssentialsX**: 基础功能扩展
- **Vault**: 经济系统支持
- **LuckPerms**: 权限管理

## 使用技巧

### 💡 效率提升
1. **合理规划领地**: 充分利用领地空间
2. **参与经济活动**: 积极交易获得资源
3. **完成每日任务**: 稳定获得奖励
4. **加入活跃公会**: 享受团队支持

### ⚠️ 注意事项
- 遵守服务器规则和社区准则
- 尊重其他玩家的财产和创作
- 合理使用高级功能，避免滥用
- 及时备份重要建筑和物品

### 🔄 定期维护
- **数据备份**: 定期备份重要数据
- **权限审查**: 检查权限设置合理性
- **性能监控**: 注意功能对服务器性能影响

---
*高级功能让游戏体验更丰富，但请记住游戏的核心还是创造和社交* 
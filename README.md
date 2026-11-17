# 归途旅装（Wayfarer Travel Kit）

《我的世界》26.3 / Forge 66 模组。一个围绕「旅装」展开的内容包：旅装三件套、三条材料线、两个世界之外的维度与遗迹、以及一套机械自动化。

## 安装

1. 安装 Forge 26.3（66.x）
2. 把 `wayfarer-26.3-2.2.4.jar` 放进 `mods` 文件夹
3. 启动游戏（首次进入会生成 `config/wayfarer-common.toml`）

## 开局三步

1. 铁锭 + 木棍做**旅者之刃**与**旅者之镐**
2. 铁锭×4 + 指南针做**归途罗盘**，右键记录第一个家
3. 用 `/sethome` 与 `/home` 随时往返

## 三条材料线

| 材料线 | 矿石位置 | 强度 |
|---|---|---|
| 熔岩 | 下界 | 与钻石齐平，抗火 |
| 虚无 | 末地主岛与外岛 | 高于下界合金，可挖基岩 |
| 星辉 | 主世界防火之地 / 遗迹 / BOSS | 高于虚无 |
| 深渊 | 第四维度「深渊」 | 高于星辉 |

## 遗迹与 BOSS

- 防火村庄、虚空神殿、熔岩神庙、深渊废墟、深渊方尖碑、工厂遗迹
- 6 个 BOSS：遗忘之王、熔岩巨兽、灰烬君王、虚空守望者、霜王、深渊巨像
- 用**召唤祭坛**配合材料召唤 BOSS

## 机械时代

线缆把发电机、电池、机器连成网络；虚无发电机烧虚无能量发电；电熔炉不用燃料；物品管道自动搬货；自动合成台按图案自动合成；传送机用锚石绑定目的地；工厂核心四周摆 8 块电池成 40 万容量的多方块。

## 新增工具

- **生物图鉴**：右键打开面板，查看全部 26 种生物的生命、攻击与掉落
- **建筑蓝图**：潜行右键记两个角点，右键把结构贴到目标位置（上限 16×16×16）
- **能量 HUD**：屏幕左上角常驻显示周围能源网络储量
- **传送锚石 / 召唤之杖 / 探矿器 / 扩容背包**

## 指令

| 指令 | 作用 |
|---|---|
| `/sethome` / `/home` | 设置 / 返回家 |
| `/back` | 回到上次死亡点 |
| `/wayfarer help` | 帮助 |
| `/wayfarer locate [village\|temple\|lava_temple\|factory\|abyss\|obelisk]` | 定位遗迹 |
| `/wayfarer bestiary` | 列出全部生物 |
| `/wayfarer energy` | 报告周围储能 |

## 配置

| 键 | 默认 | 说明 |
|---|---|---|
| `general.enableGrave` | true | 死亡是否生成墓碑 |
| `general.lowDurabilityPercent` | 15 | 低耐久提示阈值 |
| `general.compassCooldownTicks` | 600 | 罗盘冷却 |
| `general.wandCooldownTicks` | 10 | 法杖冷却 |
| `general.eliteChancePercent` | 3 | 精英怪概率 |
| `loot.starShardWeight` | 2 | 星辉碎片权重 |
| `machines.energyPerItem` | 2000 | 电熔炉每件耗电 |
| `machines.cableNodeLimit` | 512 | 能源网络节点上限 |
| `machines.pipeIntervalTicks` | 8 | 管道搬运间隔 |
| `machines.crafterIntervalTicks` | 20 | 合成台间隔 |
| `machines.factoryCoreCapacity` | 400000 | 工厂核心容量 |

## 已知限制

- 防火之地只对**新世界**生成（需要覆盖世界预设）
- 「熔岩海」是下界成片岩浆湖，不是独立群系（下界气候点没有可插入空间）
- 能量 HUD 与蓝图复制尚未实现，计划 2.1

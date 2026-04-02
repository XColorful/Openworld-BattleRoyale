# 修改地形生成配置

## 数据包
整合包加入了[OBR数据包：减少主世界植被数量](https://github.com/XColorful/OBR-less-vegetation)和[OBR数据包：增加主世界建筑数量](https://github.com/XColorful/OBR-more-structures)
- 整合包已经帮你自动在客户端/服务端加载该数据包，位于 _./minecraft/datapacks_ 下
- 如果不需要以上功能，一个简单的方式就是在游戏启动前删除数据包

## 模组
> 模组控制的村庄生成频率独立于数据包、但村庄间距离仍然生效

常见配置项：
- spacing：将地图分为若干方形网格，边长为spacing，在每个网格内尝试生成建筑
- separation：使建筑间距离不小于这个值
> _separation_ 应小于 _spacing_，单位均为区块（16格）

### 村庄
_./minecraft/config/bettervillage_1.properties_

> 整合包将村庄提供的箱子当作[自定义大逃杀](https://github.com/XColorful/BattleRoyale)的主要刷新手段，并且掩体众多，功能上相当于“城区”

### 其他建筑
_./minecraft/config/towns_and_towers_
_./minecraft/config/better……-forge-1_20.toml_
_./minecraft/config/better……-forge-1_20.toml.bak_

该类别建筑不宜过多，因为：
- 野区补给以[OBR数据包：增加主世界建筑数量](https://github.com/XColorful/OBR-more-structures)控制的废弃地狱门与沉船为主
- 平坦地形掩体以[OBR数据包：减少主世界植被数量]控制的树木为主

### 扁平地形
_./minecraft/config/tectonic.json_

> 整合包预期需要“压扁”的地形，由于TerraForge未更新1.20.1以及整合包作者没能用ReTerraForge配置调出较好的地形，最后使用[Tectonic](https://github.com/Apollounknowndev/tectonic)

- terrain\_scale：设置为 _0.05_ 与 _0.001_ 差别不大，无法再压得更扁

# English

## Datapacks
The modpack includes the following datapacks: [OBR less vegetation](https://github.com/XColorful/OBR-less-vegetation) and [OBR more structures](https://github.com/XColorful/OBR-more-structures).
- The modpack automatically loads these datapacks for you on both the client and server, located under _./minecraft/datapacks_
- If you don't need these features, a simple way to disable them is to delete the datapacks before launching the game.

## Mods
> Mod-controlled village generation frequency is independent of datapacks, but the spacing between villages still applies.

Common configuration options:
- spacing: Divides the map into square grids with side length spacing. The game attempts to generate structures within each grid.
- separation: Ensures that structures are not closer than this value.
> _separation_ should be less than _spacing_. Both units are in chunks (16 blocks).

### Villages
_./minecraft/config/bettervillage_1.properties_

> The modpack primarily uses chests provided by villages as the main loot generating method for [Custom BattleRoyale](https://github.com/XColorful/BattleRoyale). With their abundant cover, villages functionally serve as "urban areas."

### Other Structures
_./minecraft/config/towns_and_towers_
_./minecraft/config/better……-forge-1_20.toml_
_./minecraft/config/better……-forge-1_20.toml.bak_

It's not advisable to have too many structures of this category because:
- Wilderness supplies are primarily controlled by abandoned nether portals and shipwrecks, managed by the [OBR more structures](https://github.com/XColorful/OBR-more-structures).
- Cover in flat terrain is mainly provided by trees, controlled by the [OBR less vegetation](https://github.com/XColorful/OBR-less-vegetation)

### Flattened Terrain
_./minecraft/config/tectonic.json_

> This modpack aims for "flattened" terrain. Since TerraForge hasn't updated to 1.20.1 and the modpack author couldn't achieve satisfactory terrain using ReTerraForge configurations, [Tectonic](https://github.com/Apollounknowndev/tectonic) was used instead.

- terrain\_scale: Setting this to _0.05_ versus _0.001_ makes little difference; the terrain cannot be flattened further.
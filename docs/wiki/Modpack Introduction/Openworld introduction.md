# 开放世界地形

## 生成地形

整合包使用[Chunky](https://github.com/pop4959/Chunky)方便地预生成地形，只需在服务端输入如下指令：
```
/chunky center 0 0
/chunky radius 4096 4096
/chunky start
```
地形生成结束后，将区块复制到单人游戏存档内使用[JourneyMap](https://teamjm.github.io/journeymap-docs/5.9.x/)绘制大地图
> 整合包测试时固定使用种子0，实际使用随机种子即可

## 地形分类

预期的世界地形以[Tectonic](https://github.com/Apollounknowndev/tectonic)、[OBR数据包：减少主世界植被数量](https://github.com/XColorful/OBR-less-vegetation)、[OBR数据包：增加主世界建筑数量](https://github.com/XColorful/OBR-more-structures)所作的修改为主，最终地形的性质可用两种标准来判断：

### 对战环境
> 与[OBR数据包：减少主世界植被数量](https://github.com/XColorful/OBR-less-vegetation)的分类大致相同

#### 平坦地形
- 特征：树木稀少、草丛数量极少
- 代表：平原、沙漠
> 掩体少、无法隐藏，需要正面交锋

#### 树林
- 特征：树木适中、含有高草丛
- 代表：白桦林、樱花林、黑森林、热带草原
> 无法防备侧面进攻

#### 密集掩体
- 特征：树木较多、草丛数量多且隐蔽性好
- 代表：丛林、村庄（城区）
> 既危险又安全

### 物资数量
> 与[OBR数据包：增加主世界建筑数量](https://github.com/XColorful/OBR-more-structures)的分类大致相同

#### 野区
- 特征：面积广、建筑少
- 代表：平原、沙漠（实际均显示为深海）
> 物资少，不作为获取物资的主要手段

#### 城区
- 特征：所在群系面积小、建筑多
- 代表：村庄
> 提供丰富物资的同时容易埋伏，交战时掩体过多

#### 豪宅
- 特征：单独分布，物资集中
- 代表：林地府邸
> 高价值目标，可能引发激烈争夺

# English

## Generating Terrain

This modpack uses [Chunky](https://github.com/pop4959/Chunky) for convenient pre-generation of terrain, just use the following commands on the server:
```
/chunky center 0 0
/chunky radius 4096 4096
/chunky start
```
After terrain generation is complete, copy the chunks to your single-player save and use [JourneyMap](https://teamjm.github.io/journeymap-docs/5.9.x/) to render the large map.
> The modpack was tested using a fixed seed of 0, but you can use a random seed for actual play.

## Terrain Categorization

The expected world terrain is primarily influenced by modifications made by [Tectonic](https://github.com/Apollounknowndev/tectonic), [OBR less vegetation](https://github.com/XColorful/OBR-less-vegetation), and [OBR more structures](https://github.com/XColorful/OBR-more-structures). The nature of the final terrain can be judged by two standards:

### Combat Environment
> Roughly similar to the categorization in [OBR less vegetation](https://github.com/XColorful/OBR-less-vegetation).

#### Flat Terrain
- Characteristics: Sparse trees, very few bushes.
- Examples: Plains, Deserts.
> Provides little cover, making direct confrontations unavoidable.

#### Forest
- Characteristics: Moderate tree density, contains tall grass.
- Examples: Birch Forests, Cherry Groves, Dark Forests, Savannas.
> Offers limited protection from flanking attacks.

#### Dense Cover
- Characteristics: Many trees, abundant and well-concealed bushes.
- Examples: Jungles, Villages (Urban Areas).
> Both dangerous and safe due to numerous hiding spots.

### Loot Quantity
> Roughly similar to the categorization in [OBR more structures](https://github.com/XColorful/OBR-more-structures).

#### Wilderness
- Characteristics: Vast area, few structures.
- Examples: Plains, Deserts (often appear as deep oceans in-game).
> Sparse loot, not intended as a primary source of supplies.

#### Urban Areas
- Characteristics: Small biome area, many structures.
- Examples: Villages.
> Provides abundant loot but also offers many ambush opportunities; combat here can involve excessive cover.

#### Mansion
- Characteristics: Isolated distribution, concentrated high-value loot.
- Examples: Woodland Mansions.
> High-value targets that may lead to intense contests.
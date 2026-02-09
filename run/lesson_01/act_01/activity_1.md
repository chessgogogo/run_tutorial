### @activities true

## Introduction
### Step 1: 欢迎
@showdialog
# 欢迎来到 Minecraft Education 教程
欢迎来到 Minecraft Education，你将学习如何使用 MakeCode 积木编程来创建 Minecraft 中的自动化功能。

让我们开始第一个任务：当游戏开始时，给自己一把镐子！

## Activity 1: 给予玩家工具
### Step 2: 创建开机给予镐子
现在我们将创建一个程序，当游戏开始时自动给予最近的玩家一把镐子。

按照以下步骤操作：

1. 从 **循环** 分类中拖出 **当开机时** 积木
2. 从 **生物** 分类中拖出 **提供给** 积木，放入 **当开机时** 积木内部
3. 从 **方块** 分类中拖出 **镐子** 积木，放入 **方块或物品** 椭圆形框内
4. 在 **提供给** 积木中设置：
   - 目标：**最近的玩家 (@p)**
   - 物品：**镐子**
   - 数量：**1**



```blocks    
mobs.give(
mobs.target(NEAREST_PLAYER),
WOODEN_PICKAXE,
1
)
```
﻿## 入队logs查询插件
### 注意：LOGS不代表玩家真实水平，请不要通过LOGS做出影响其他玩家正常游戏的行为。

这里是一个入队播报 logs的ACT插件，

基本的工作原理是： 当检测到有玩家加入队伍时，调用fflogs提供的接口，读取你所指定的副本的logs，然后播报其最高的logs值，并且在悬浮窗上显示出来。

#### 基于此原理，你需要
 1. 指定apiKey - 用于调用fflogs接口
 2. 指定区域 - 例如伊甸、欧米茄、或者讨伐高难，不指定则默认当前版本高难本(伊甸)
 3. 指定副本BOSS - 例如虚无行者、利维亚桑或者泰坦，不指定则从当前选择的区域中列举全部BOSS，并播报其中最高的一个logs
 4. 指定你所在的服务器 - 玩家入队时如果玩家名不带服务器名，则使用这个服务器查询
 5. 使用ACT中ngld悬浮窗插件，并添加一个适用于显示logs信息的模板（我已经开发了一个默认的）



#### 可以开关控制的功能
 * 整体功能启用
 * 入队自动检测
 * 输入 /e logs 玩家名查询 (例如 /e logs  &lt;2&gt; 可以查询2号队员)
 * 语音播报

[悬浮窗以及语音播报效果 av81965841](https://www.bilibili.com/video/av81965841/)
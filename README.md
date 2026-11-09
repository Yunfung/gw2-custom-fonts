# 激战2 自定义字体 / GW2 Custom Fonts

《激战2》(Guild Wars 2) 中使用的中文字体文件备份与说明。

## 文件清单

| 文件 | 大小 | 字体 | 字重 | 许可 |
| --- | --- | --- | --- | --- |
| `jiangcheng-yuanti 600W.ttf` | 14.39 MB | 江城圆体 600W（JiangChengYuanTi） | 600 | SIL OFL 1.1 |
| `LXGWWenKaiMonoGB-B2.ttf` | 57.65 MB | 霞鹜文楷等宽 GB **加粗2**（基于 LXGW WenKai Mono GB Medium，轮廓外扩 r=6，family 霞鹜文楷等宽 GB 加粗2） | 700 | SIL OFL 1.1 |
| `SourceHeiSansSC-Bold.otf` | 16.18 MB | 思源黑体 Bold（Source Han Sans SC Bold） | 700 | SIL OFL 1.1 |

三款字体均为 SIL Open Font License 1.1，可自由使用、修改与再分发，再分发时请保留原许可声明。

## 关于「加粗2」

- 由 LXGW WenKai Mono GB Medium 做轮廓等距外扩（radius = 6/1000 em）生成，未缩放、未改 advance。
- 度量保持原样：upem 1000、advance 1000、asc/desc 928/-241，所以字形不会互相挤压。
- 体积 23.52 MB → 57.65 MB：曲线被离散成折线，属正常代价。
- 闸值参考：同源三档在 22px 下的墨量分别为 +5.2%（r3）/ +11.6%（r6）/ +15.4%（r9），r6 是中间的「加粗2」。

## 使用方式（Scruffy FontKit）

1. 把插件装到 `Guild Wars 2/addons/`。
2. 游戏内 `Esc → Addons → Scruffy FontKit`。
3. `Choose font...` 选择 ttf/otf，再点 `Build font pack`（约 40 秒 ~ 数分钟，生成 ~700 MB 缓存，可边玩边等）。
4. 重启后若仍要求重建，检查 `addons/scruffy-fontkit/build/font.pack.key` 是否写入成功。

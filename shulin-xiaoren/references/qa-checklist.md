# QA Checklist

## 必过项

- 是 16:9 横版
- 背景是干净纯白底
- 有罗小森
- 罗小森的发色是浅暖金/奶黄色（不是纯白、不是铂金）
- 罗小森有粗黑框矩形眼镜，眼睛正常大小可见（不是豆豆眼）
- 灯泡是泪滴形白炽灯，绳索连灯顶，向下悬挂（不是提灯/手电筒/LED）
- 罗小森承担核心动作，不只是装饰
- 没有复刻旧案例构图，为当前内容生成了新隐喻
- 画面怪诞、有创意、有意思
- 简洁清爽，主体不超过画面约 55%
- 一张图只讲一个核心结构
- 中文标注少、短、能读（最多 5 个，每个 2-6 字）
- 橙色只用于主路径或箭头
- 红色只用于重点、问题、提醒或结果
- 蓝色只用于补充说明或系统状态
- 琥珀/暖黄仅用于灯泡光芒（如有），不超过 3-4 根细线

## 失败信号 → 处理方式

| 问题 | 处理 |
|---|---|
| 豆豆眼 / 两个小点眼睛 | 重生成，加"NOT tiny dot eyes, NOT bean eyes, normal chibi eyes with brown irises" |
| 灯泡变成提灯/手电筒/圆球 | 重生成，加"teardrop incandescent bulb, cord at crown, hangs downward, NOT lantern NOT flashlight" |
| 发色变成纯白/铂金 | 重生成，加"light warm blonde, cream-yellow, NOT pure white, NOT platinum" |
| 眼镜消失或变圆框/细框 | 重生成，加"thick solid rectangular black frames, slightly oversized, must be visible" |
| 风衣细节消失变纯黑色块 | 重生成，加"visible lapels, front buttons, brown belt with silver buckle, coat hem" |
| 罗小森只是装饰 | 重写 Scene，让罗小森执行核心动作 |
| 画面像 PPT / 正式流程图 | 去掉标题、边框、整齐网格，改成手绘场景 |
| 左上角有类型标题 | 局部编辑删除，或重生成时强调"no title in top-left corner" |
| 中文标注不可读 | 减少至 2-3 个短标注，重生成 |
| 背景有纹理/阴影/渐变 | 重生成，加"pure white background only, no texture, no shadow, no gradient" |
| 画面太满 | 删元素，只保留核心动作和 1-2 个主物件 |

## 交付判断

高质量图应该让读者先觉得"有点怪"，然后 1 秒内看懂结构。

如果第一眼像教程页，而不是白纸上的怪诞产品草图，就不合格。

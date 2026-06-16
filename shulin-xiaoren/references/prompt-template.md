# 生图提示词模板

每张图单独生成。根据正文内容替换变量，不要把多张图拼在一起。

## 固定开头（每张图必须包含）

```text
Generate one standalone 16:9 horizontal Chinese article illustration. Pure white background. Minimalist hand-drawn sketch composition — wobbly rough pen lines for objects, paths, annotations. Lots of empty white space, subject 40-55% of canvas. Sparse handwritten Chinese annotations. No gradients, no shadows, no paper texture, no PPT look, no commercial illustration style.

Recurring character 罗小森: chibi proportions, large head compact body. Clean confident ink line art — more refined than the rough environment. Fluffy layered light warm blonde / pale golden-yellow hair (cream-yellow, NOT pure white, NOT platinum), slightly tousled with visible individual strands. Thick rectangular black-framed glasses (NOT round, NOT thin wire frames — thick solid rectangular frames, slightly oversized). Eyes: normal chibi-sized eyes with visible dark brown irises, defined upper eyelid line, subtle lower lash line. NOT tiny dot eyes. NOT bean-shaped mini eyes. NOT two small dots. Eyes clearly visible behind the glasses lenses — warm, slightly heavy-lidded, calm gaze. Long black trench coat with lapels, front button placket, brown leather belt with silver buckle, coat hem reaching below the knee. Black turtleneck scarf: loosely wrapped around neck, fabric visibly bunched and layered with natural draping folds. White shirt collar visible at chest opening. Black straight-leg trousers. Black leather lace-up boots, ankle height, slightly chunky sole with visible lace eyelets.

Signature prop — Edison bulb (MUST match this exact description every time):
Classic teardrop-shaped incandescent bulb. Clear glass dome (wider at bottom, narrowing to a neck at top). Inside the glass: a coiled tungsten filament, clearly visible. Short cylindrical copper/brass screw socket at the very bottom of the bulb. A thin black cord/wire attaches to the CROWN (very top) of the bulb — the character holds the cord, letting the bulb HANG downward. NOT held by the base. NOT a lantern. NOT a flashlight. NOT a modern LED bulb shape. When lit: warm amber-golden glow from the filament, 3-4 thin straight radiating lines extending outward. When unlit: no glow, filament still visible inside clear glass.

Expression — pick the one that best fits the scene concept:
- 认真 (focused): slight frown, intent gaze directly at the task, fully absorbed
- 轻傲 (quietly proud): one corner of mouth slightly raised, calm superiority, like the outcome was obvious
- 微笑 (cool smile): small closed-mouth smile, relaxed, not cute — more knowing than warm
- 好奇 (curious): head slightly tilted, one eyebrow raised behind glasses, studying something intently
- 无奈 (wry/resigned): slight downward mouth corners, composed but mildly exasperated, the look of "here we go again"
- 若有所思 (pensive): gaze drifting slightly off to the side, lips lightly pursed, quietly thinking
- 满意 (quietly satisfied): eyes slightly narrowed with contentment, small upward lip, like watching a plan come together
- 困惑 (puzzled): one eyebrow visibly higher than the other behind the glasses frames, head barely tilted
- 坚定 (determined): direct forward gaze, chin level, jaw set, no hesitation
- 淡漠 (detached): eyes half-lidded, gaze slightly averted, complete composed indifference
Always cool and collected. No rosy cheeks, no sparkly eyes, no wide open mouth, no tears.

Color: black for all line art and 罗小森. Orange for main flow/arrows. Red for key warnings/results. Blue for secondary notes. Warm amber ONLY for Edison bulb glow lines.
```

---

## 场景变量（每张图替换这部分）

```text
Expression: {从上方10种表情中选一种，写明英文描述}

Scene: {具体画面：罗小森在哪里、正在做什么、灯泡是亮还是灭、主要物件是什么、信息如何流动}

Chinese handwritten labels: {标注词1} / {标注词2} / {标注词3}（最多5个，每个2-6字）

Structure type: {Workflow / 系统局部 / 前后对比 / 角色状态 / 概念隐喻 / 方法分层 / 地图路线 / 小漫画分镜}
```

---

## 图像编辑提示

**去掉左上角标题：**

```text
Edit the provided image. Remove only the handwritten title "{要删除的文字}" and its underline from the top-left corner. Fill that area with clean white background matching the surrounding area. Preserve everything else exactly: characters, labels, paths, line style, composition, aspect ratio. Do not add any new text or objects.
```

**加强罗小森参与感：**

```text
Regenerate with the same core meaning and layout. Make 罗小森 the active subject of the conceptual action — pushing, holding the bulb up to illuminate something, getting stuck, pulling, sorting. Not standing to the side. Keep the character's clean ink line quality. Edison bulb must be visible and match the teardrop hanging-cord style.
```

**人物眼睛变成豆豆眼时：**

```text
Regenerate. Keep the same composition and concept. Fix 罗小森's eyes: they must be normal chibi-sized eyes with visible dark brown irises and defined eyelid lines — NOT tiny dots, NOT bean eyes, NOT two small circles. Eyes should be clearly visible behind the rectangular glasses frames, warm and slightly heavy-lidded.
```

**灯泡样式跑偏时：**

```text
Regenerate. Keep the same composition. Fix the Edison bulb: it must be a classic teardrop-shaped incandescent bulb with clear glass dome, visible coiled tungsten filament inside, copper screw socket at the bottom, thin black cord attached to the very TOP of the bulb. The character holds the cord so the bulb hangs downward. NOT a lantern, NOT a torch, NOT a modern LED bulb.
```

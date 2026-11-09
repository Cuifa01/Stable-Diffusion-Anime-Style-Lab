# Myonstyle v2｜生图框架（讨论稿）

本文件保存本人提供的原始生成框架及固定参数，用于后续讨论 v2 训练素材的变量设计。**目前仅为讨论稿，不是可直接批量执行的配置。**

- 方括号 `[ ]`：固定内容，讨论过程中未经确认不修改。
- 花括号 `{ }`：可变内容，目前仅为原始示例，候选池尚未确定。
- `BREAK`：保留原有六段式顺序。
- Seed 使用花括号，表示不同生成任务可以更换；其余生成参数均沿用下方记录。
- 方括号、花括号是文档标记，不应连同括号原样提交给 NeoForge。
- 目标流程：250 张候选图 → 人工筛选 120 张 → 100 张训练 + 20 张保留检验；v1 原有 45 张不混入。**本文件暂不决定变量、训练或测试生成任务。**

## 原始示例（逐字保留）

~~~text
[masterpiece,best quality,highres,newest,ultra detailed,detailed face,beautiful color,sfw,loli,solo,]
BREAK
{from side, upper body, looking at viewer, tilted composition}
BREAK
{holding gohei,holding staff,finger to cheek,hand on own cheek,head tilt,looking at viewer,}
BREAK
{kochiya sanae,smile,closed mouth,blush,gentle smile,
windblown hair,side braid,frog hair ornament,snake hair ornament,}
[blush,body blush,shiny skin,]
BREAK
{shrine maiden,white shirt,white blouse,sleeveless shirt,wide sleeves,
blue frilled skirt,}
[slender,]
BREAK
[artist:tianliang duohe fangdongye,(kanpa \(campagne 9\):0.8),(alpha \(alpha91\):0.6),(koyama shigeru:0.6),(massakasama:0.55),<lora:nyalia:0.6>,]
BREAK
[simple background,white background,white border,
sky,cloudy sky,sunset,sunset lighting,soft lighting,]
[Negative prompt: western comics \(style\),realistic,nsfw,text,extra digits,extra toes,bad feet,lowres,jpeg artifacts,bad anatomy,bad hands,worst quality,low quality,signature,watermark,blurry,cropped,multiple views,anthro,chibi inset,monochrome,boldline,<lora:noobaiXL_EasyNegative_LoRA-3.0_last:1>,
Steps: 15, Sampler: Kohaku LoNyu Yog, Schedule type: Karras, CFG scale: 3.5,]{ Seed: 1871366906,} [Size: 832x1152, Model: waiNSFWIllustrious_v150, Model hash: befc694a29, Module 1: sdxl_vae, Denoising strength: 0.2, RNG: GPU, ADetailer model: 99coins_anime_girl_face_m_seg.pt, ADetailer prompt: "flat color, blush, ", ADetailer negative prompt: "western comics \\(style\\), realistic, sweat,", ADetailer confidence: 0.3, ADetailer method to decide top k masks: Area, ADetailer mask only top k: 1, ADetailer dilate erode: 4, ADetailer mask blur: 4, ADetailer denoising strength: 0.5, ADetailer inpaint only masked: True, ADetailer inpaint padding: 32, ADetailer Version: Neo, Hires Module 1: Use same choices, Hires upscale: 1.5, Lora hashes: "nyalia: 965D9B2AB486", Emphasis: No norm, Hires upscaler: 4xNMKDSuperscale_4xNMKDSuperscale, Hires steps: 12, Hires CFG Scale: 3, Version: neo-2.26]
~~~

## 当前讨论边界

本次只保留原样，不将示例中的角色、服装、视角、动作、表情、背景或光照提前定为最终变量组合。后续按模块逐项讨论，再由本人确认是否修改本文件。

# Myonstyle v1｜训练数据

**正式训练数据：45 张 SFW 图片与 45 份同名 Caption。** 已完成图文配对检查。

素材使用 WAI-Illustrious v15、原始画师串与 nyalia LoRA 生成，人工筛选经过 Hires.fix、面部 ADetailer 的成品。最初规划 165 张候选，早期初选 43 项，正式训练集为 45 对文件；计划数量不代表实际生成量。

## 角色与构图

初期计划覆盖 11 个角色：东方 Project 的妖梦、四季映姬、魔理沙、古明地觉、古明地恋、琪露诺、蕾米莉亚、芙兰朵露，以及 Blue Archive 的鬼方佳代子、阿罗娜、天童爱丽丝。

构图计划包括脸部特写、3/4 视角、半身、腰部构图和轻动态姿势。角色的最终入选数量以本地数据集为准，不能直接从计划推断。

## 标注

早期使用 WD14 `wd-vit-v3` 辅助打标，初选阈值 `0.5`。正式 AI Toolkit 训练使用触发词 `myonstyle`。Caption 是否全部完成了逐条人工修订，尚无完整核验记录。

本地路径：`D:\AI_painting\Training\Datasets\Myon_style`。

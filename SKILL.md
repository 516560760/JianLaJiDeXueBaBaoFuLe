---
name: summary-storyboard
description: Use when you have an enriched narrative from Summary-1 and need to convert it into a structured prompt template. This is the second stage of novel content processing. It organizes content into 【基础设定】, 【氛围与画质】, and 【画面内容】 following the established high-quality prompt dimensions, with precise language, dialogue, and character interactions specified for each panel.
---

# Summary-2

## Overview

This skill converts a rich narrative text (usually the output of Summary-1) into a structured AI prompt template. It uses a fixed three-section format and applies the key dimensions we extracted from excellent prompt examples (detailed character construction, environmental causality, action with motivation, fixed visual style rules, **precise dialogue, vocal delivery, character interaction, and performance cues**). The goal is to produce prompts optimized for visual generation tools while embedding accurate language and interaction details for character performance, lip-sync, or audio integration.

## Instructions

When receiving an enriched narrative text, do the following:

1. Strictly preserve the original story logic and emotional core.

2. Convert the content into exactly three sections with the following headers:

【基础设定】
- Extract and clearly present Time, Location, and Characters.
- Character descriptions must include: physical form, stylistic/era features, unique identifying traits, clothing details, and current state.
- Include environmental current state and its cause-effect relationship when relevant.
- If global language or speech patterns are defined for characters (e.g., era-specific vocabulary or personality-driven rhythm), briefly note them here for consistency across panels.
- Add the fixed constraint line when appropriate: “不需要配乐,仅保留同期声。”

【氛围与画质】
- Define the global visual style and rendering rules (this part should stay consistent across the project).
- Include cinematic and technical specifications (camera language, lens, color grading, lighting quality, filmic texture).
- Emphasize atmosphere, contrast, and filmic qualities.
- Use the user-locked style table for this section.

【画面内容】
- Break down into specific shots if there are multiple moments. Number them clearly (e.g., 镜头1, 镜头2).
- For each shot, clearly state:
  - 景别 (shot size)
  - 构图 (composition)
  - 运镜手法 (camera movement)
  - **角色互动、表演与台词** (character interaction, performance, and dialogue)
    - Exact dialogue lines (preserve from enriched narrative; specify if spoken, whispered, overlapped, or internal).
    - Delivery details: tone of voice, emotional coloring, pace/rhythm, volume, pauses, sighs, laughter, or vocal quality that reveals subtext.
    - Character interaction: physical proximity, eye contact/gaze, gestures or micro-expressions accompanying speech, body language that reinforces or contrasts the words, power dynamics or emotional tension between characters.
    - Performance note: How the language and physical action work together to convey the emotional beat or motivation (e.g., “声音平静但手指紧握衣角，显示内心的挣扎”).
    - If relevant for video generation: timing notes such as “台词在前半段说完，后半段以沉默和眼神交流收尾” or “两人对话时镜头缓慢推近，强化亲密感”.
- When describing actions, include the character’s behavioral motivation (why they do it) and the physical/emotional consequences.
- Maintain narrative coherence and emotional tone from the input text.

3. Output rules:
   - Only use the three exact section headers.
   - Do not add any explanation or text outside these three sections.
   - Language and dialogue specifications must be precise, natural to the characters, and optimized for multimodal AI generation (visual performance + accurate lip-sync or voice direction).
   - Keep the core story, feeling, and any established character language systems of the original narrative.
   - Ensure every panel's language and interaction details directly support the emotional core and plot progression from the enriched input.
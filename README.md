# wenyanwen

中文 | English

## 中文介绍

`wenyanwen` 是一个偏向高密度、少废话、工具式回答的 Codex skill。

它的核心思路不是把最终回答都写成文言文，而是尽量用中文文言式骨架来压缩内部任务整理、问题抽取、计划草案和中间摘要；真正展示给用户的回答，默认仍使用用户当前的语言，并保持正常、清楚、简洁。

适合这类场景：

- 希望回答更短、更快、更直接
- 希望减少寒暄、铺垫、重复总结
- 希望默认采用结论优先、信息密度更高的表达
- 希望像 `原始人.skill` 一样追求节省 token，但外部输出仍然自然可读

默认行为：

- 对用户可见的最终回答：跟随用户语言，正常表达
- 对用户不可见的内部压缩与整理：尽量使用中文文言式骨架
- 只有在用户明确要求时，最终回答才会真的使用文言文

注意：

- 这是 prompt/style 层面的约束，不是可证明的底层推理改写
- 它可能帮助减少冗余输出，但不保证精确节省多少 token

## English

`wenyanwen` is a Codex skill for terse, high-density, utility-first responses.

Its main idea is not to make the visible answer sound like classical Chinese. Instead, it encourages a compressed classical-Chinese-style internal scaffold for task shaping, plan drafts, problem reduction, and intermediate summaries, while keeping the final user-facing answer in the user's normal language.

This skill is a good fit when you want:

- shorter, faster, more direct answers
- less filler, less politeness padding, and less repetition
- answer-first structure with higher information density
- a style similar to `primitive-man.skill`, but with normal outward language

Default behavior:

- User-facing output stays in the user's language and reads normally
- Internal compression and planning lean toward a classical-Chinese-style scaffold
- Actual classical-Chinese output is only used when the user explicitly asks for it

Notes:

- This is a prompt/style constraint, not a provable low-level reasoning rewrite
- It may reduce redundant output, but it does not guarantee a specific token saving

## Files

- [SKILL.md](./SKILL.md): main skill definition
- [agents/openai.yaml](./agents/openai.yaml): UI metadata

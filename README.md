Inducing AI to Slack Off: Default Narrative Persona and Deviation Strategy

Supplementary materials for "Inducing AI to Slack Off: Default Narrative Persona and Bounded Freedom in Deviation Strategies for Large Language Models" (arXiv, 2026).

目录结构 / Directory Structure

plaintext
├── 提示词/                         # Prompts
│   ├── 征酱完整提示词.txt           # 偏离策略完整提示词
│   ├── 去A/B/C/D-消融实验提示词
│   └── 孔子测试原文存档.txt
├── 测试数据/                       # Test Data (压缩包自取 / see zip archives)
│   ├── deepseek/ChatGPT/Grok/豆包/千问/
│   └── 消融实验原始输出
└── paper-en.tex                    # 论文LaTeX源码


消融实验 / Ablation Scores

表格
Condition	Layers	Score	Root Cause
Full version	A+B+C	9.0	Gap Lock non-mutual-exclusion
Remove A	B+C	5.5	Drifted to "non-unique index"
Remove B	A+C	8.5–9.0	Gap Lock (almost no loss)
Remove C	A+B	Failed	Four voices exploded
Remove fear	A\feared+B+C	7–7.5	RR/current read confusion

Citation

bibtex
@article{zhang2026deviation,
  title={Inducing AI to Slack Off: Default Narrative Persona and Bounded Freedom in Deviation Strategies for Large Language Models},
  author={WeiXianZhang},
  year={2026},
  eprint={XXXX.XXXXX},
  archivePrefix={arXiv}
}


License

MIT

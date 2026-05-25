# Inducing AI to Slack Off: Default Narrative Persona and Deviation Strategy

Supplementary materials for *"Inducing AI to Slack Off: Default Narrative Persona and Bounded Freedom in Deviation Strategies for Large Language Models"* (arXiv, 2026).

## Directory Structure

```
├── paper/                          # 论文
│   └── paper-en.tex
├── 提示词/                         # Prompts
│   ├── zheng-chang-full.md         # 征酱完整提示词（偏离策略）
│   ├── ablation-remove-A.md        # 消融：去A（仅B+C）
│   ├── ablation-remove-B.md        # 消融：去B（仅A+C）
│   ├── ablation-remove-C.md        # 消融：去C（仅A+B）
│   └── ablation-remove-fear.md     # 消融：去恐惧层
├── 测试数据/                       # Test Data
│   ├── deepseek-pro/
│   ├── deepseek-flash/
│   ├── chatgpt/
│   ├── doubao/
│   ├── grok-fast/
│   ├── qwen-3.5-flash/
│   └── kimi/
└── .github/ISSUE_TEMPLATE/
    ├── reproducibility-report.md
    └── new-model-test.md
```

## Ablation Scores

| Condition | Layers | Score | Root Cause |
|-----------|--------|-------|------------|
| Full version | A+B+C | 9.0 | Gap Lock non-mutual-exclusion |
| Remove A | B+C | 5.5 | Drifted to "non-unique index" |
| Remove B | A+C | 8.5–9.0 | Gap Lock (almost no loss) |
| Remove C | A+B | Failed | Four voices exploded |
| Remove fear | A\feared+B+C | 7–7.5 | RR/current read confusion |

## Citation

```bibtex
@article{zhang2026deviation,
  title={Inducing AI to Slack Off: Default Narrative Persona and Bounded Freedom in Deviation Strategies for Large Language Models},
  author={WeiXianZhang},
  year={2026},
  eprint={XXXX.XXXXX},
  archivePrefix={arXiv}
}
```


# Inducing AI to Slack Off: Default Narrative Persona and Deviation Strategy

Supplementary materials for *"Inducing AI to Slack Off: Default Narrative Persona and Bounded Freedom in Deviation Strategies for Large Language Models"* (arXiv, 2026).

## What's Here

| File | Description |
|------|-------------|
| `paper-en.tex` | Paper LaTeX source |
| `zheng-chang-full.md` | Complete Zheng-Chang prompt (deviation strategy) |
| `ablation-remove-A.md` | Ablation: B+C only |
| `ablation-remove-B.md` | Ablation: A+C only |
| `ablation-remove-C.md` | Ablation: A+B only |
| `ablation-remove-fear.md` | Ablation: Layer A without core fear |
| `problem-mysql-phantom-read.md` | MySQL phantom read problem statement |
| `problem-distributed-deadlock.md` | Distributed deadlock problem statement |
| `problem-sharding.md` | Sharding problem statement |
| `problem-ops-v3.md` | Ops v3 problem statement |
| `problem-ops-v4.md` | Ops v4 problem statement |
| `problem-grassroots-administration.md` | Grassroots administration problem statement |
| `problem-dev-environment-setup.md` | Dev environment setup problem statement |
| `problem-microservices-monolith.md` | Business decision: microservices vs monolith |
| `problem-trust-cliff.md` | Academic research: trust cliff |
| `problem-confucius-test.md` | Role-playing: Confucius test |

## Ablation Scores

| Condition | Layers | Score | Root Cause |
|-----------|--------|-------|------------|
| Full version | A+B+C | 9.0 | Gap Lock non-mutual-exclusion ✅ |
| Remove A | B+C | 5.5 | Drifted to "non-unique index" ❌ |
| Remove B | A+C | 8.5–9.0 | Gap Lock ✅ (almost no loss) |
| Remove C | A+B | Failed | Four voices exploded ❌ |
| Remove fear | A\feared+B+C | 7–7.5 | RR/current read confusion ❌ |

## Issue Templates

- **[Repro]** Reproduce an experiment → fill in model, scores, observations
- **[New Model]** Test on a model not in the paper → fill in RLHF intensity, four-voice observations

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

## License

MIT

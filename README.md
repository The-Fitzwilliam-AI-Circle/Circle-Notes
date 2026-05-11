# Circle Notes

Session notes, reading summaries, and discussion documentation for The Fitzwilliam AI Circle.

**Duration:** February–November 2026
**Location:** Dublin, Ireland

---

## About

This repository contains our collective documentation as we work through questions about how AI systems can support scientific discovery when feedback is sparse, expensive, or uncertain.

Three core questions guide the programme:

1. **Verification under uncertainty** — When ground truth is unavailable, what proxy signals can guide learning?
2. **Research taste as a learnable capability** — Can AI systems learn to judge which problems are worth pursuing?
3. **Exploration without exploitation** — Can AI systems explore like creative humans without mode collapse?

---

## Repository Structure

```
circle-notes/
├── month-01-foundations/
├── month-02-training/
├── month-03-reasoning/
├── ...
└── resources/
```

Each monthly folder contains:
- Session notes
- Reading summaries and discussion questions
- Any outputs or artefacts from that month

---

## Reading List

> **Note:** Readings for months past June are tentative and may be changed as the programme develops.

### Month 0 — Primer Materials

*Complete before the programme begins.*

#### Understanding Neural Networks

- [A short introduction to machine learning](https://www.alignmentforum.org/posts/qE73pqxAZmeACsAdF/a-short-introduction-to-machine-learning)
- [But what is a neural network?](https://www.youtube.com/watch?v=aircAruvnKk) (video)
- [Gradient descent, how neural networks learn](https://www.youtube.com/watch?v=IHZwWFHWa-w) (video)

#### Understanding Transformers & LLMs

- [Intro to Large Language Models](https://www.youtube.com/watch?v=zjkBMFhNj_g) (video)
- [But what is a GPT? Visual intro to transformers](https://www.youtube.com/watch?v=wjZofJX0v4M) (video)
- [The Illustrated Transformer](http://jalammar.github.io/illustrated-transformer/)

#### Scaling & Big Picture Context

- [The Bitter Lesson](http://www.incompleteideas.net/IncIdeas/BitterLesson.html)
- [Scaling Laws for Neural Language Models](https://arxiv.org/abs/2001.08361)

#### Optional

- [Attention in transformers, visually explained](https://www.youtube.com/watch?v=eMlx5fFNoYc) (video)
- [Attention? Attention!](https://lilianweng.github.io/posts/2018-06-24-attention/)
- [An introduction to deep reinforcement learning](https://thomassimonini.medium.com/an-introduction-to-deep-reinforcement-learning-17a565999c0c)

---

### Month 1 — April: Foundations

*Foundation model architectures — how do modern LLMs work?*

**Reading group:** Saturday, April 25th, 3pm
**Technical lab:** Thursday, April 30th, 6pm — implementing GPT-1 from scratch

#### Core

- Vaswani et al. (2017), [Attention is All You Need](https://arxiv.org/abs/1706.03762)
- Radford et al. (2018), [Improving Language Understanding by Generative Pre-Training](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf)
- Radford et al. (2019), [Language Models are Unsupervised Multitask Learners](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)

#### Bonus

- Andrej Karpathy, [Deep Dive into LLMs like ChatGPT](https://www.youtube.com/watch?v=7xTGNNLPyMI) (video)

#### Supplemental

- [The Illustrated GPT-2](https://jalammar.github.io/illustrated-gpt2/)
- [DeepSeek-V3 Technical Report](https://arxiv.org/abs/2412.19437)

---

### Month 2 — May: Scaling

*How do scaling laws shape what we build, and what falls out when you take compute seriously?*

**Reading group:** Saturday, May 16th, 3pm

#### Core

- Kaplan et al. (2020), [Scaling Laws for Neural Language Models](https://arxiv.org/abs/2001.08361)
- Brown et al. (2020), [Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165)
- Hoffmann et al. (2022), [Training Compute-Optimal Large Language Models](https://arxiv.org/abs/2203.15556)

#### Bonus

- Richard Sutton, [The Bitter Lesson](https://www.cs.utexas.edu/~eunsol/courses/data/bitter_lesson.pdf)

#### Supplemental

- [Training language models to follow instructions with human feedback](https://arxiv.org/abs/2203.02155) (InstructGPT)
- [Learning to summarize from human feedback](https://arxiv.org/abs/2009.01325)
- [Direct Preference Optimization](http://arxiv.org/abs/2305.18290)
- [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685)
- [QLoRA: Efficient Finetuning of Quantized LLMs](http://arxiv.org/abs/2305.14314)

---

### Month 3 — June: Reasoning

*Chains of thought and reasoning models — how do we get models to reason?*

#### Core

- [Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/pdf/2201.11903)
- [Solving math word problems with process- and outcome-based feedback](https://arxiv.org/pdf/2211.14275)
- [DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning](https://arxiv.org/pdf/2501.12948)

#### Bonus

- [Scaling LLM Test-Time Compute Optimally](https://arxiv.org/pdf/2408.03314)

#### Supplemental

- [Large Language Models are Zero-Shot Reasoners](https://arxiv.org/abs/2205.11916)
- [Self-Consistency Improves Chain of Thought Reasoning in Language Models](https://arxiv.org/abs/2203.11171)
- [s1: Simple test-time scaling](https://arxiv.org/abs/2501.19393)
- [Large Language Models Cannot Self-Correct Reasoning Yet](https://arxiv.org/abs/2310.01798v1)

---

> The readings below are **tentative** and subject to change.

### Month 4 — July: Decomposition

*Breaking complex problems into tractable pieces.*

#### Core

- [Supervise Process, not Outcomes](https://ought.org/updates/2022-04-06-process)
- [Tree of Thoughts: Deliberate Problem Solving with Large Language Models](http://arxiv.org/abs/2305.10601)
- [Iterated Distillation and Amplification](https://ai-alignment.com/iterated-distillation-and-amplification-157debfd1616)

#### Supplemental

- [Factored Verification: Detecting and Reducing Hallucination in Summarization](https://arxiv.org/abs/2310.10627)
- [Training Verifiers to Solve Math Word Problems](https://arxiv.org/abs/2110.14168)
- [Recursively Summarizing Books with Human Feedback](https://arxiv.org/abs/2109.10862)

---

### Month 5 — August: Agents

*Tool use, code execution, agentic scaffolding.*

#### Core

- [WebGPT: Browser-assisted question-answering with human feedback](https://arxiv.org/abs/2112.09332)
- [Executable Code Actions Elicit Better LLM Agents](https://arxiv.org/abs/2402.01030)
- [AI capabilities can be significantly improved without expensive retraining](http://arxiv.org/abs/2312.07413)

#### Supplemental

- [Measuring the impact of post-training enhancements](https://metr.github.io/autonomy-evals-guide/elicitation-gap/)
- [TextGrad: Automatic "Differentiation" via Text](https://arxiv.org/abs/2406.07496)
- [DSPy: Compiling Declarative Language Model Calls into Self-Improving Pipelines](http://arxiv.org/abs/2310.03714)
- [Voyager: An Open-Ended Embodied Agent with Large Language Models](http://arxiv.org/abs/2305.16291)

---

### Month 6 — September: Applications

*LLMs applied to scientific discovery.*

#### Core

- [AlphaEvolve: A coding agent for scientific and algorithmic discovery](https://arxiv.org/abs/2506.13131)
- [Accurate structure prediction of biomolecular interactions with AlphaFold 3](https://www.nature.com/articles/s41586-024-07487-w)
- [The Impact of Large Language Models on Scientific Discovery](http://arxiv.org/abs/2311.07361)

#### Supplemental

- [Towards an AI Co-Scientist](https://storage.googleapis.com/deepmind-media/DeepMind.com/Blog/towards-an-ai-co-scientist/Towards_an_AI_Co-Scientist.pdf)
- [Can large language models provide useful feedback on research papers?](http://arxiv.org/abs/2310.01783)
- [Large Language Models Encode Clinical Knowledge](http://arxiv.org/abs/2212.13138)
- [Automated Statistical Model Discovery with Language Models](http://arxiv.org/abs/2402.17879)

---

### Month 7 — October: Uncertainty

*Quantifying and communicating model uncertainty.*

#### Core

- [Teaching Models to Express Their Uncertainty in Words](https://arxiv.org/abs/2205.14334)
- [Experts Don't Cheat: Learning What You Don't Know By Predicting Pairs](http://arxiv.org/abs/2402.08733)
- [Approaching Human-Level Forecasting with Language Models](http://arxiv.org/abs/2402.18563)

#### Supplemental

- [Textual Bayes: Quantifying Uncertainty in LLM-Based Systems](https://arxiv.org/abs/2506.10060)
- [TruthfulQA: Measuring How Models Mimic Human Falsehoods](https://arxiv.org/abs/2109.07958)
- [What Evidence Do Language Models Find Convincing?](http://arxiv.org/abs/2402.11782)
- [Consistency Checks for Language Model Forecasters](https://arxiv.org/abs/2412.18544)

---

### Month 8 — November: Interpretability

*What is going on in there?*

#### Core

- [Scaling Monosemanticity: Extracting Interpretable Features from Claude 3 Sonnet](https://transformer-circuits.pub/2024/scaling-monosemanticity/)
- [Discovering Latent Knowledge in Language Models Without Supervision](https://arxiv.org/abs/2212.03827v1)
- [Representation Engineering: A Top-Down Approach to AI Transparency](http://arxiv.org/abs/2310.01405)

#### Supplemental

- [A Mathematical Framework for Transformer Circuits](https://transformer-circuits.pub/2021/framework/index.html)
- [Language Models Represent Space and Time](http://arxiv.org/abs/2310.02207)
- [Emergent World Representations](http://arxiv.org/abs/2210.13382)
- [Opening the AI black box: program synthesis via mechanistic interpretability](https://arxiv.org/abs/2402.05110v1)

---

### Month 9 — December: Discovery

*Paradigms for scientific discovery.*

#### Core

- [Mastering Chess and Shogi by Self-Play with a General Reinforcement Learning Algorithm](https://arxiv.org/abs/1712.01815) (AlphaZero)
- [Mastering Atari, Go, Chess and Shogi by Planning with a Learned Model](https://arxiv.org/abs/1911.08265) (MuZero)
- [Reflexion: Language Agents with Verbal Reinforcement Learning](http://arxiv.org/abs/2303.11366)

#### Supplemental

- [Decision Transformer: Reinforcement Learning via Sequence Modeling](https://arxiv.org/abs/2106.01345)
- [Open Problems and Fundamental Limitations of Reinforcement Learning from Human Feedback](http://arxiv.org/abs/2307.15217)
- [Solving olympiad geometry without human demonstrations](https://www.nature.com/articles/s41586-023-06747-5)
- [AlphaStar: Mastering the Real-Time Strategy Game StarCraft II](https://deepmind.com/blog/article/alphastar-mastering-real-time-strategy-game-starcraft-ii)

---

### Month 10 — January: Synthesis

*No new readings. Focus on consolidation, writing, and the closing symposium.*

---

## Contributing

Session notes should be added to the relevant monthly folder. Use the filename format `session-NN-topic.md`.

Reading summaries can be added as separate files or appended to session notes where they were discussed.

---

## Links

- [Workshops repository](https://github.com/The-Fitzwilliam-AI-Circle/Workshops) — Notebooks and code for technical sessions
- [Experiments repository](https://github.com/The-Fitzwilliam-AI-Circle/Experiments) — Exploratory experiments
- [The Fitzwilliam](https://thefitzwilliam.com/ai-circle) — Programme updates and blog posts

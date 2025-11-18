<div align="center">

# PromptBridge: Cross-Model Prompt Transfer for Large Language Models

<a href='https://github.com/supergirl-os/PromptBridge'><img src='https://img.shields.io/badge/Project-Page-Green'></a>
<a href='https://www.arxiv.org/pdf/2410.11143'><img src='https://img.shields.io/badge/Paper-PDF-orange'></a> 

Large language models (LLMs) underpin applications in code generation, mathematical reasoning, and agent-based workflows. In practice, systems access LLMs via commercial APIs or open-source deployments, and the model landscape (e.g., GPT, Claude, Llama) evolves rapidly. This rapid evolution forces frequent model switches driven by capability, cost, deployment constraints, and privacy. Yet prompts are highly model-sensitive: reusing a prompt engineered for one model on another often yields substantially worse performance than a prompt optimized for the target model. We term this phenomenon \emph{Model Drifting}. Through extensive empirical analysis across diverse LLM configurations, we show that model drifting is both common and severe.
To address this challenge, we introduce \emph{PromptBridge}, a training-free framework that preserves prompt effectiveness under model switches, enabling cross-model prompt transfer without costly per-task or per-model re-optimization. PromptBridge requires only a small set of alignment tasks for calibration. It first applies \emph{Model-Adaptive Reflective Prompt Evolution (MAP-RPE)} to obtain task- and model-specific optimal prompts via iterative reflective refinement and quantitative evaluation. Using the resulting calibrated prompt pairs for the source and target models, PromptBridge learns a cross-model prompt mapping. At test time, i.e., for an unseen task, given a source-model prompt, this mapping directly produces an optimized prompt for the target model.
Experiments in single-LLM, single-agent, and multi-agent settings show that PromptBridge consistently improves downstream accuracy while reducing migration effort. For example, when transferring from \texttt{GPT-4o} to \texttt{o3}, PromptBridge yields a 27.39\% improvement on \textsc{SWE-Bench} and a 39.44\% improvement on \textsc{Terminal-Bench} relative to direct transfer. These results establish cross-model prompt transferability as a critical requirement for sustainable LLM system development and demonstrate that PromptBridge is an effective, practical, training-free solution for maintaining performance as models evolve.

</div>


## 🎉🎉 News 
<!-- - [x] [2025.01] 👏👏 Accepted by **ICLR 2025**. -->
- [x] [2025.11] 🚀🚀 Release the paper of [**PromptBridge**](https://github.com/supergirl-os/PromptBridge).

## The code will be availiable soon!
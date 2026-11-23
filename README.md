<div align="center">
 <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:FFFDF7,35:FDF6E3,70:F5EBCD,100:EED9B7&height=200&section=header&text=Pierre%20Ramez%20Francis&fontSize=46&fontColor=111111&fontAlign=50&fontAlignY=36&desc=Evaluating%20and%20Serving%20LLMs%20for%20Code&descAlign=50&descAlignY=58&descSize=15&descColor=222222&animation=fadeIn"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=2600&pause=900&color=B8860B&center=true&vCenter=true&width=900&lines=Evaluating+LLMs+for+code;Mutation+testing+with+LLMs;LLM+agents+for+software+engineering;Serving+LLMs+on+constrained+hardware)](https://github.com/pr-francis)

<br>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/pierreramez)
&nbsp;
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:pierre.ramez10@gmail.com)
&nbsp;
[![GitHub](https://img.shields.io/badge/GitHub-0D1117?style=flat-square&logo=github&logoColor=white)](https://github.com/pr-francis)

<sub>MSA University × University of Greenwich &nbsp;·&nbsp; 6th of October, Egypt &nbsp;·&nbsp; Graduating June 2027</sub>

</div>

<br>

---

### About

I work on large language models for code, mostly on whether their results hold up when you check them. Since June 2026 I have been an undergraduate researcher in the [UIUC++ Summer Research in Software Engineering (SRSE)](https://uiuc-srse.github.io/) program, which I joined through a Verus evaluation task. There I work on LLM-based mutation testing, a survey on discrete diffusion for code generation, and two empirical software-engineering studies.

My graduation project uses a contextual bandit to decide when a code model should retrieve context. I am now moving toward the engineering side of this work, the systems that run and serve these models efficiently. From February to June 2026 I was an AI intern at [ControlPoint](https://control-point.io/about), an OT/ICS cybersecurity startup, where I reviewed agentic AI architectures for a planned product.

---

### Research Focus

- Evaluation of LLMs for code, including execution-based and mutation-based evaluation and the validity of benchmarks and test harnesses.
- LLM agents for software engineering, such as agents that read or run a project before deciding whether a mutant is equivalent.
- Efficient inference and serving on constrained hardware, from 4-bit quantization to running a 7B code model on a single T4 GPU.

---

### Now

| | Role | Where | Focus |
|--|--|--|--|
| 🔬 | **Undergraduate Researcher** | UIUC++ SRSE 2026 | LLM-based mutation testing, a survey on diffusion models for code, empirical SE studies |
| 🎓 | **Graduation Project** | MSA University × University of Greenwich | AdaptCode, bandit-driven retrieval for code generation |

---

### Selected Work

<details open>
<summary><b>🔬 UIUC++ SRSE Research</b></summary>

<br>

- Found a selector leak in the group's mutation-testing pipeline that let LLM-generated tests read which mutant was running and earn kill credit without checking behaviour. I fixed it across the JavaScript, Java and C runners with regression tests. Five of my pull requests to the pipeline are merged.
- Lead writer of the formal and neuro-symbolic verification section in a survey on discrete diffusion for code generation, with every claim checked against the source papers and their released code.
- Audited the bug-report claims of three papers for the ISSTA 2026 paper [*The Discreet Charm of the Bugeoisie*](https://doi.org/10.1145/3832244), where I am acknowledged.
- Reviewed about 1,040 Stack Overflow posts, GitHub issues and contest problems for a dataset of real ambiguities in software requirements.

</details>

<br>

<details open>
<summary><b>🎯 AdaptCode: Code Generation with Bandit-Driven Adaptive RAG</b> &nbsp;<em>(Graduation Project)</em></summary>

<br>

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![vLLM](https://img.shields.io/badge/vLLM-30A2FF?style=flat-square)
![Qwen2.5-Coder](https://img.shields.io/badge/Qwen2.5--Coder_7B-615CED?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

A contextual bandit (LinUCB, Thompson Sampling) chooses for each query whether and where to retrieve context, and its reward is whether the generated code passes its tests in a sandbox. I own the retrieval layers, the bandit algorithms and the experiments. In the first full DS-1000 evaluation, about 7,000 completions from Qwen2.5-Coder-7B served with vLLM in 4-bit AWQ on a single T4 GPU, generating with no retrieval was the strongest single setting, so it is the baseline any adaptive policy has to beat.

</details>

<br>

<details open>
<summary><b>🤖 Ouro: Closed-Loop Active Learning System</b> &nbsp;<em>(Team Lead)</em></summary>

<br>

![Llama](https://img.shields.io/badge/Llama_3.2_3B-1a1a2e?style=flat-square)
![Unsloth](https://img.shields.io/badge/Unsloth-ff6b35?style=flat-square)
![LoRA](https://img.shields.io/badge/LoRA-6c3483?style=flat-square)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
[![Repo](https://img.shields.io/badge/Repository-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/pr-francis/PersonalChatbot)

A continual-learning system built on Llama 3.2 3B. User corrections collected at inference time trigger LoRA adapter retraining, and the new adapter is hot-swapped into the running FastAPI service without a restart. Trained on a curated 13k-row dataset (DailyDialog plus a mental-health corpus), it reaches 4.08 perplexity and 0.88 BERTScore F1 on a held-out set. We chose the 3B model over Llama 3.1 8B after comparing both on the same held-out set, and 4-bit quantization cut memory use by 60% for edge deployment. Runs are tracked in MLflow, with CI on GitHub Actions.

</details>

<br>

<details open>
<summary><b>🔒 Automated OT/ICS Threat Intelligence Pipeline</b></summary>

<br>

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_2.5-4285F4?style=flat-square&logo=google&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/CI-2088FF?style=flat-square&logo=githubactions&logoColor=white)
[![Repo](https://img.shields.io/badge/Repository-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/pr-francis/Automated-Threat-Intelligence-Pipeline)

A pipeline that polls the National Vulnerability Database for new CVEs and picks out the ones relevant to OT/ICS environments. A keyword prefilter narrows the feed, then a single LLM call per CVE classifies its OT relevance and explains the likely operational impact in a fixed JSON schema. Results appear in an analyst-facing Streamlit dashboard, and a GitHub Actions workflow runs a Bandit security scan, flake8 and a functionality test on every push. This project preceded my internship at ControlPoint.

</details>

---

### Stack

<div align="center">

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Machine Learning and LLMs**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![vLLM](https://img.shields.io/badge/vLLM-30A2FF?style=flat-square)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

**MLOps and Systems**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

</div>

---

### Writing

**[A Mathematical Breakdown of Gradient Descent](https://www.linkedin.com/posts/cse-innovation-hub-msa_gradient-descent-algorithm-activity-7290795656426749952-l3WJ)**
&nbsp;·&nbsp; *CSE Innovation Hub, MSA University · Feb 2025*

A derivation of gradient descent from first principles, covering the partial derivatives of the loss, how the learning rate affects convergence, and the batch, stochastic and mini-batch variants.

---

<div align="center">

### Connect

Open to research and engineering work on LLMs for code and the systems that serve them.

📧 [pierre.ramez10@gmail.com](mailto:pierre.ramez10@gmail.com) &nbsp;·&nbsp; 💼 [linkedin.com/in/pierreramez](https://linkedin.com/in/pierreramez)

</div>

<br>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:FFFDF7,35:FDF6E3,70:F5EBCD,100:EED9B7&height=120&section=footer"/>

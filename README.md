<div align="center">
 <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:FFFDF7,35:FDF6E3,70:F5EBCD,100:EED9B7&height=200&section=header&text=Pierre%20Ramez%20Francis&fontSize=46&fontColor=111111&fontAlign=50&fontAlignY=36&desc=Reliable%20LLM%20Systems%20for%20Code%20and%20Security%2C%20under%20Real%20Constraints&descAlign=50&descAlignY=58&descSize=15&descColor=222222&animation=fadeIn"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=2600&pause=900&color=B8860B&center=true&vCenter=true&width=900&lines=LLM4Code+%3A+reliable%2C+secure+code+generation;Agentic+AI+systems+%3A+architecture+and+evaluation;Efficient+inference+on+constrained+hardware;AI+for+OT%2FICS+cybersecurity)](https://github.com/pr-francis)

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

I build LLM-based systems for software engineering and security, organized around a single question: how do you make a model's output reliable enough to trust in constrained, safety-critical settings? My work runs from formal evaluation of LLM-generated code, to agentic pipelines for industrial threat intelligence, to efficient inference on limited hardware.

In summer 2026 I am joining the [University of Illinois Summer Research in Software Engineering (UIUC++ SRSE)](https://uiuc-srse.github.io/) 2026 cohort to work on a code generation research project, after being selected through a Verus-based formal-verification evaluation. Earlier in 2026 I was an AI Intern at [ControlPoint](https://control-point.io/about), an OT/ICS cybersecurity startup, where I designed agentic architectures for industrial threat intelligence. At MSA University I lead the research group at the CSE Outstanding Hub.

---

### Research Focus

- **LLMs for code generation.** Reliable and secure code synthesis for non-trivial tasks, evaluated formally and empirically rather than by demo.
- **Agentic AI systems.** Architecture, reliability, and evaluation of autonomous LLM pipelines: task decomposition, tool use, and output contracts.
- **Efficient inference.** Quantization and principled quality-versus-cost tradeoffs for deployment on constrained hardware.
- **AI for cybersecurity.** Vulnerability analysis and automated threat intelligence for OT/ICS environments.

---

### Now

| | Role | Where | Focus |
|--|--|--|--|
| 🔬 | **Undergraduate Researcher** | UIUC++ SRSE 2026 | Code generation research; Mutation Testing; Bug Reports |
| 🧠 | **Head of Research** | Outstanding Hub, CSE Dept., MSA University *(since Nov 2025)* | Leading a research group and survey on automation in AI/ML systems |

---

### Selected Work

<details open>
<summary><b>🔒 Automated OT/ICS Threat Intelligence Pipeline</b></summary>

<br>

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_2.5-4285F4?style=flat-square&logo=google&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/CI%2FCD-2088FF?style=flat-square&logo=githubactions&logoColor=white)
[![Repo](https://img.shields.io/badge/Repository-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/pr-francis/Automated-Threat-Intelligence-Pipeline)

An agentic pipeline for industrial cybersecurity. It polls the National Vulnerability Database for live CVE feeds, applies a two-stage classifier (a domain-specific keyword prefilter, then a single LLM pass under strict JSON output contracts), and surfaces findings through an analyst-facing Streamlit dashboard, deployed via GitHub Actions. This work preceded and shaped my internship at ControlPoint.

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

A continual-learning system built on Llama 3.2 3B. A human-in-the-loop pipeline captures correction signals at inference time, triggers LoRA adapter retraining, and hot-swaps weights with no service interruption, so the model improves in production without redeployment. Trained on a 13k-row curated dataset (DailyDialog plus a mental-health corpus), it reaches 4.08 perplexity and 0.88 BERTScore F1 on a held-out set. The choice of 3B over 8B came from a controlled comparison under an identical protocol, documented as an efficiency-versus-quality tradeoff under 4-bit quantization for edge deployment. MLflow tracking and GitHub Actions throughout.

</details>

---

### Stack

<div align="center">

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

**Machine Learning and LLMs**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)

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

A derivation of gradient descent from first principles: partial derivatives of the loss function, the effect of learning rate on convergence geometry, and the Batch, Stochastic, and Mini-Batch variants.

---

<div align="center">

### Connect

Open to research collaboration in LLM systems, agentic AI, and software engineering for AI.

📧 [pierre.ramez10@gmail.com](mailto:pierre.ramez10@gmail.com) &nbsp;·&nbsp; 💼 [linkedin.com/in/pierreramez](https://linkedin.com/in/pierreramez)

</div>

<br>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:FFFDF7,35:FDF6E3,70:F5EBCD,100:EED9B7&height=120&section=footer"/>

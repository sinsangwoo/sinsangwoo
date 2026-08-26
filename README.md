<h1 align="center">Hi, I'm Sangwoo Sin 👋</h1>

<p align="center">
  <b>Freshman Software Engineering Student @ Ajou University</b><br/>
  <i>Solo-building ML/physics-simulation projects outside coursework — in short, intense bursts, not a steady grind.</i>
</p>

<p align="center">
  <a href="mailto:aksrkd7191@gmail.com">
    <img src="https://img.shields.io/badge/Email-aksrkd7191%40gmail.com-333333?style=flat-square&logo=gmail&logoColor=white"/>
  </a>
  &nbsp;
  <img src="https://img.shields.io/badge/Ajou%20University-0055A4?style=flat-square&logo=graduation-cap&logoColor=white"/>
  &nbsp;
  <img src="https://komarev.com/ghpvc/?username=sinsangwoo&style=flat-square&color=blue" alt="profile views"/>
</p>

---

## 🧭 About Me

1st-year Software Engineering student at Ajou University (started March 2026). Every project below is solo, unreleased, and unstarred — built to learn something specific, not to ship a product. Development happens in bursts: a few weeks of daily commits on one repo, then months of nothing, then a burst on the next one.

- 🔬 What I've actually built so far: gradient-diagnostics tooling, PDE solvers (FNO/PINN), classical-ML-vs-GNN experiments, a chest X-ray classifier prototype, and a from-scratch OS scheduler/memory simulator
- 🏥 Where I'm aiming, not where I am: medical imaging and industrial-process ML — nothing shipped there yet, still building the fundamentals
- 📐 How I actually work: derive or read the paper before importing the library. Most performance numbers in the projects below are self-measured inside each repo, not independently verified — flagged explicitly there rather than left to imply more than they show

---

## 🚀 Featured Projects

### 🔧 ML Tooling & Research

| Project | What it is | Stack |
|:---|:---|:---|
| **[Gradient Pathology](https://github.com/sinsangwoo/Why_Isnt_It_Learning)** | PyTorch library that profiles gradient statistics during training to catch vanishing/exploding gradients and dead neurons — layer-wise heatmaps, Sankey diagrams, a live Streamlit dashboard, and a 7-rule diagnostic engine with code-fix suggestions. Has tests and an in-repo benchmark (under ~3% training overhead). Zero stars, zero outside users — a solo tool, not an adopted library. | `PyTorch` `Plotly` `Streamlit` `Python` |
| **[Physics-Informed ML](https://github.com/sinsangwoo/Physics-Informed-ML)** | Fourier Neural Operator and PINN implementations for the heat equation, Burgers', and Navier-Stokes, wrapped in a FastAPI backend and a React/Three.js 3D frontend, plus uncertainty-quantification experiments (Bayesian PINN, deep ensembles). The "100–1000× faster than solvers" number compares a trained model's inference time to a full classical solve — a self-reported, in-repo comparison, not a third-party benchmark. | `PyTorch` `FastAPI` `React` `Three.js` `Terraform` |
| **[ML Gradient Descent Viz](https://github.com/sinsangwoo/ML-Gradient-Descent-Viz)** | Started as a from-scratch NumPy backprop/MLP implementation, grew into a small optimizer library (SGD through AdamW) with convergence-theory notes and JAX/CuPy GPU benchmarks. The "deep non-convex" phase mentioned in the repo is still unbuilt — everything working today is convex/near-convex. | `NumPy` `JAX` `Python` |
| **[Physics-Informed Optimizer](https://github.com/sinsangwoo/Physics-Informed-Optimizer)** | JAX/Flax framework for solving PDEs with physics-informed neural nets (heat equation, Navier-Stokes) — PINN-specific training tricks (curriculum learning, adaptive loss balancing), multi-GPU training, a Streamlit dashboard. Despite the name, it's not a general-purpose optimizer that uses physical priors; it's a PDE solver. | `Python` `JAX` `Flax` |
| **[Chemical Reaction Rate Prediction](https://github.com/sinsangwoo/Chemical-Reaction-Rate-Prediction-ML)** | Started as a high-school chemistry class project. Now compares RandomForest/XGBoost against GNNs (GCN, GAT, GIN, MPNN) for predicting reaction rates from molecular structure, with a FastAPI + React interface. Headline numbers in the repo (R² 0.985, +18% from a hybrid model) are self-reported from commit messages, not from a published or independently reproduced result. | `Scikit-learn` `PyTorch (GNN)` `FastAPI` `React` |

### 🌐 Web & Systems

| Project | What it is | Stack |
|:---|:---|:---|
| **[Ajou Dorm Finder](https://github.com/sinsangwoo/ajou-dorm-finder)** | Unofficial dorm-eligibility checker and assignment-score calculator for Ajou University students, with per-semester facility data, room-type charts, and a countdown to the new dorm building. No backend — all data is hardcoded per semester and updated by hand. | `React` `TypeScript` `Vite` |
| **[AI Disease Classifier](https://github.com/sinsangwoo/AIdiseaseclassifier)** | Chest X-ray pneumonia-classification prototype — Flask API, ONNX Runtime inference, Grad-CAM heatmaps for explainability. The ONNX step is a format conversion, not quantization; there's no training code in the repo to back a class-imbalance fix. The project's own README already flags it as an educational prototype with no FDA/CE clearance. | `Flask` `ONNX` `JavaScript` |
| **[Mini OS Simulator](https://github.com/sinsangwoo/mini-os-sim)** | CLI simulator of process scheduling (FCFS, SJF, Round Robin, Priority), paging and page replacement (FIFO/LRU), and syscalls (SLEEP/IO/FORK/EXIT) — built to learn OS fundamentals by implementing them, not to run anything real. | `Python` `C` |
| **[NPU Simulator](https://github.com/sinsangwoo/NPU_Simulator)** | Repo created, nothing committed yet. Listed as an open placeholder for a hardware-inference-acceleration idea I haven't started, not as finished work. | — |

### 📝 NLP & Data

| Project | What it is | Stack |
|:---|:---|:---|
| **[AI Cyberbullying NLP Analysis](https://github.com/sinsangwoo/AI-Cyberbullying-NLP-Analysis)** | One-day project: TF-IDF + scikit-learn classifier for Korean toxic-comment detection, trained on 80k rows sampled from an AI Hub ethics dataset. No transformer model — that's future work noted in the README, not something built. | `Python` `Scikit-learn` |

---

## 🛠 Tech Stack

| Category | Technologies |
|:---|:---|
| **Languages** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) |
| **ML & Science** | ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white) ![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white) ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white) |
| **Backend & APIs** | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white) ![ONNX](https://img.shields.io/badge/ONNX-005CED?style=flat-square&logo=onnx&logoColor=white) |
| **Frontend** | ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=three.js&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) |
| **DevOps & Cloud** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) |

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=sinsangwoo&show_icons=true&theme=default&hide_border=true&count_private=true" height="150"/>
  &nbsp;
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=sinsangwoo&layout=compact&theme=default&hide_border=true" height="150"/>
</p>

---

## 📖 Education

| Period | Institution | Details |
|:---|:---|:---|
| 2023 – 2025 | **Eunhye High School** | — |
| 2026 – | **Ajou University** | B.S. Software Engineering · AI · Industrial Engineering · Bio-Informatics |

---

## 📝 TIL

Learning log at **[sinsangwoo/TIL](https://github.com/sinsangwoo/TIL)** — notes on algorithms, ML theory, and tools, capped at 5 lines a day. Automated and daily since mid-August 2026; before that there's a 5-month gap where nothing was written.

---

<div align="center">
  <sub>16 public repos, 0 stars — each built to learn one thing, not to ship. That part's next.</sub>
</div>

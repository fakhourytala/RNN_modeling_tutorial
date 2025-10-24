# Rule-Guided Sequence Planning with RNNs
**Reproducing PFC-like, rank-ordered working-memory “slot” dynamics and strategy adaptation**

This notebook trains recurrent neural networks (RNNs) to model **rule-dependent sequence planning**, inspired by macaque **PFC/PMd** population activity in a multi-step, abstract-rule task. It also includes a **meta-RL** variant to infer **policies/values** and detect **strategy shifts** when task parameters change.

---

## TL;DR
- **Goal:** Model how **abstract rules** are transformed into **rank-ordered WM “slots”** and maintained for sequential control; connect model states to neural-style population geometry.
- **Core:** Train an RNN (optionally low-rank) on a **3-step rule task**; evaluate **slot representations**, **cross-temporal decoding**, and a **communication-subspace** proxy.
- **Extras:** A **meta-RL** version that infers monkey-like **policy/strategy shifts** under task changes.

---

## Repository
- `train_rnn.ipynb` — end-to-end notebook: data generation → model → training → analysis → plots  
- *(optional)* `data/` — drop real/sim data here  
- *(optional)* `models/` — saved weights / checkpoints  
- *(optional)* `figs/` — generated figures

> The project is notebook-first; you can later refactor helpers into `src/`.

---

## Environment
Tested on **Python 3.10+**.

**Install (conda + pip example):**
```bash
conda create -n seqwm python=3.10 -y
conda activate seqwm
pip install -r requirements.txt



Contact
Tala Fakhoury - tf2546@columbia.edu — Center for Theoretical Neuroscience, Columbia

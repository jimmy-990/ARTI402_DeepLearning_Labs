## Lab 4 — Recurrent Networks: RNN, LSTM and GRU

This lab implements an RNN cell and an LSTM cell from scratch in NumPy and counts the parameters of an RNN, a GRU and an LSTM. It then tests how long each model remembers the first step.

**Results:** with the same frozen weights, the RNN forgot step 1 within about 5 steps. The LSTM scored 0.942 at T=40, and a forget bias of +4 was the best setting.

**Files:** `arti402_Lab4_2240005270.ipynb`, `arti402_figures.py`

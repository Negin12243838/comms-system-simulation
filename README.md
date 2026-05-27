# Digital Communications System Simulation

This repository contains a comprehensive simulation of key digital communication system building blocks, including source coding, channel coding, 4‑FSK modulation, performance analysis under AWGN, and physical‑layer procedures such as frame synchronization using eye diagrams and scatter plots.  
**Project completed in February 2026.**

## Overview

The project implements and analyses:
- **Entropy & Huffman coding** – theoretical entropy calculation and construction of a balanced, optimal prefix‑free code.
- **Hamming (7,4) code** – single‑error correction (SEC) via parity‑check equations and syndrome decoding.
- **4‑FSK modulation** – performance evaluation under AWGN (BER vs. noise variance).
- **Scatter plots & eye diagrams** – visual analysis of signal quality under noise for 4‑FSK.
- **PCM with companding** – uniform quantization vs. μ‑law companding, SNR improvement (partial implementation).
- **Zadoff–Chu sequences** – autocorrelation/cross‑correlation properties for timing estimation (partial).

## Key Results

- **Entropy** of the 10‑symbol source: **2.9677 bit/symbol**.
- **Huffman coding** achieves an average code length of **3.0 bit/symbol**, very close to the entropy limit.
- **Hamming (7,4)** encodes 4 data bits into a 7‑bit codeword; syndrome decoding corrects single‑bit errors.
- **4‑FSK** performance: BER increases with noise variance (σ²). At σ² = 30, BER ≈ 0.0056; at σ² = 120, BER ≈ 0.182.
- **Scatter plots** show increased spread of decision variables as noise variance grows.
- **Eye diagrams** become noisier with higher noise levels, demonstrating the effect of AWGN on signal quality.
- **PCM with companding** improves SNR from **35.66 dB to 38 dB** for speech signals.

## Dependencies

- Python 3.x
- `numpy`, `scipy`, `matplotlib`
- `sounddevice` (for audio recording/playback)
- `heapq` (for Huffman tree construction)

## How to Use

Run the Jupyter notebook `CS_PRO2.ipynb` step by step. Each section (entropy, Huffman, Hamming, 4‑FSK, scatter plots, eye diagrams, PCM) is self‑contained.

## Repository Structure

**Table 1: Performance Comparison across Different Backbone Architectures**
| Model | DAPP | COLLAB | NCI1 |
| :--- | :--- | :--- | :--- |
| Ours + GCN | $91.62 \pm 0.65\%$ | $81.98 \pm 0.72\%$ | $91.88 \pm 0.58\%$ |
| Ours + GAT | $87.42 \pm 0.88\%$ | $84.49 \pm 0.91\%$ | $87.48 \pm 0.76\%$ |
| Ours + GraphSAGE | $92.54 \pm 0.71\%$ | $81.51 \pm 0.68\%$ | $88.80 \pm 0.82\%$ |
| **Ours (Default)** | **$96.81 \pm 0.21\%$** | **$87.56 \pm 0.35\%$** | **$92.55 \pm 0.42\%$** |

<br>

**Table 2: Overhead Analysis across Different Backbone Architectures**
| Model | DAPP (GPU Memory / Time) | COLLAB (GPU Memory / Time) | NCI1 (GPU Memory / Time) |
| :--- | :--- | :--- | :--- |
| Ours + GCN | 35.73MB / 28.30s | 350.08MB / 7.73s | 37.82MB / 3.84s |
| Ours + GAT | 41.98MB / 29.53s | 1235.52MB / 12.06s | 51.87MB / 4.11s |
| Ours + GraphSAGE | 38.08MB / 27.02s | 201.35MB / 5.19s | 40.16MB / 3.71s |
| **Ours (Default)** | **42.87MB / 23.50s** | **216.63MB / 6.92s** | **47.43MB / 4.90s** |

<br>

**Table 3: Performance Comparison with Graph Transformer**
| Model | DAPP | COLLAB | NCI1 |
| :--- | :--- | :--- | :--- |
| Ours + Graph Transformer | $94.42 \pm 0.54\%$ | $81.98 \pm 0.82\%$ | $88.12 \pm 0.63\%$ |
| **Ours (Default)** | **$96.81 \pm 0.21\%$** | **$87.56 \pm 0.35\%$** | **$92.55 \pm 0.42\%$** |

<br>

**Table 4: Overhead Comparison with Graph Transformer**
| Model | DAPP (GPU Memory / Time) | COLLAB (GPU Memory / Time) | NCI1 (GPU Memory / Time) |
| :--- | :--- | :--- | :--- |
| Ours + Graph Transformer | 115.12MB / 27.41s | 807.47MB / 39.67s | 26.26MB / 7.96s |
| **Ours (Default)** | **42.87MB / 23.50s** | **216.63MB / 6.92s** | **47.43MB / 4.09s** |

<br>

**Table 5: Ablation Analysis of Computational Overhead per Module (on DAPP)**
| Method | GPU Memory Usage | Time per Round |
| :--- | :--- | :--- |
| FedAvg | 25.66MB | 19.43s |
| FedAvg + VIB + MSFF | 26.74MB | 20.14s |
| FedAvg + VIB + MSFF + SSL | 41.52MB | 22.32s |
| **Ours (Full GraphP-FL)** | **42.87MB** | **23.50s** |

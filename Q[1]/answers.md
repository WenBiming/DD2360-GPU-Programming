# Explain in your own words three main architectural differences between GPUs and CPUs
- GPU is math-intensive device, having relatively more computational units and less control units
- GPU has better parallel capability, designed for parallel compuatational tasks, with hardware-level mutithreading
- CPU employs SingleInstruction, Multiple Data (SIMD) execution, while GPU employs Single-Instruction,Multiple Threads (SIMT) execution.


# Summary of Top 10 Super Computers

**Only one system (Fugaku)** does *not* use GPUs/accelerators.
**The other 9 systems use GPU/accelerator hardware.**

Here is the summary:

| Rank | System Name                      | GPU / Accelerator Vendor | Model                              |
| ---- | -------------------------------- | ------------------------ | ---------------------------------- |
| 1    | **El Capitan**                   | **AMD**                  | **Instinct MI300A**                |
| 2    | **Frontier**                     | **AMD**                  | **Instinct MI250X**                |
| 3    | **Aurora**                       | **Intel**                | **Data Center GPU Max Series**     |
| 4    | **JUPITER Booster**              | **NVIDIA**               | **GH200 (Grace Hopper Superchip)** |
| 5    | **Eagle (Microsoft Azure NDv5)** | **NVIDIA**               | **H100**                           |
| 6    | **HPC6**                         | **AMD**                  | **Instinct MI250X**                |
| 7    | **Supercomputer Fugaku**         | **(No GPU)**             | Uses Fujitsu **A64FX CPU** only    |
| 8    | **Alps**                         | **NVIDIA**               | **GH200 (Grace Hopper Superchip)** |
| 9    | **LUMI**                         | **AMD**                  | **Instinct MI250X**                |
| 10   | **Leonardo**                     | **NVIDIA**               | **A100 (SXM4)**                    |

### **Answer**

* **Number of systems with GPUs in the TOP 10:** **9 out of 10**
* **Only Fugaku does not use GPUs.**



# Power Efficiency of Top 10 Super Computers
Perfect — since the **June 2025** list page *does include both Rmax and Power* for the Top 10, we can directly compute **power efficiency** now.

The efficiency metric is:

$$
\textbf{GFLOPS/W} = \frac{R_{\text{max}}(\text{PF})}{\text{Power (kW)}} \times 1000
$$

---



|   Rank | System                   | GPU / Accelerator                        | Rmax (PFLOPS) |       Power (kW) | **GFLOPS/W** |
| -----: | ------------------------ | ---------------------------------------- | ------------: | ---------------: | -----------: |
|  **1** | **El Capitan** (USA)     | **AMD Instinct MI300A**                  |       1742.00 |           29,581 |   **≈ 58.9** |
|  **2** | **Frontier** (USA)       | **AMD Instinct MI250X**                  |       1353.00 |           24,607 |   **≈ 55.0** |
|  **3** | **Aurora** (USA)         | **Intel Data Center GPU Max**            |       1012.00 |           38,698 |   **≈ 26.2** |
|  **4** | **JUPITER Booster** (DE) | **NVIDIA GH200 Grace Hopper**            |        793.40 |           13,088 |   **≈ 60.6** |
|  **5** | **Eagle** (USA)          | **NVIDIA H100**                          |        561.20 | **Not Reported** |      **N/A** |
|  **6** | **HPC6** (Italy)         | **AMD Instinct MI250X**                  |        477.90 |            8,461 |   **≈ 56.5** |
|  **7** | **Fugaku** (Japan)       | **Fujitsu A64FX (CPU SIMD)** *(no GPUs)* |        442.01 |           29,899 |   **≈ 14.8** |
|  **8** | **Alps** (Switzerland)   | **NVIDIA GH200 Grace Hopper**            |        434.90 |            7,124 |   **≈ 61.0** |
|  **9** | **LUMI** (Finland)       | **AMD Instinct MI250X**                  |        379.70 |            7,107 |   **≈ 53.4** |
| **10** | **Leonardo** (Italy)     | **NVIDIA A100 SXM4**                     |        241.20 |            7,494 |   **≈ 32.2** |

---




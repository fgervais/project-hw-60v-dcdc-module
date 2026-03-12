# 4.3V to 60V input / 0.8V to 30V output switching converter

- [PCB v1.0.0-5-g07f53f4](#pcb-v100-5-g07f53f4)
  - [Switching converter analysis](#switching-converter-analysis)
    - [Switch node](#switch-node)
  - [Output (5V, 2x 10uF 50V output capacitors)](#output-5v-2x-10uf-50v-output-capacitors)
  - [Output (5V, 2x 22uF 16V output capacitors)](#output-5V-2x-22uF-16V-output-capacitors)
- [PCB v1.0.0-5-g07f53f4 (hack1)](#pcb-v100-5-g07f53f4-hack1)
  - [Switching converter analysis](#switching-converter-analysis-lmr51625)
  - [Output (5V, 2x 22uF 16V output capacitors)](#output-5V-lmr51625-2x-22uF-16V-output-capacitors)

## PCB v1.0.0-5-g07f53f4

### Switching converter analysis

![Overview](assets/img/sw_node_overview.jpg)

50 ohms series termination at the SW node.

![Closeup](assets/img/sw_node_closeup.jpg)

#### Switch node

| Input Voltage | Waveform | Rising edge |
|---------------|----------|-------------|
| 10V           | ![Waveform](assets/img/sw_node_10V_400mA/DS2_QuickPrint96.png) | ![Rising](assets/img/sw_node_10V_400mA/DS2_QuickPrint97.png) |
| 20V           | ![Waveform](assets/img/sw_node_20V_400mA/DS2_QuickPrint98.png) | ![Rising](assets/img/sw_node_20V_400mA/DS2_QuickPrint99.png) |
| 48V           | ![Waveform](assets/img/sw_node_48V_500mA/DS2_QuickPrint100.png) | ![Rising](assets/img/sw_node_48V_500mA/DS2_QuickPrint102.png) |

### Output (5V, 2x 10uF 50V output capacitors)

![Probe Setup](assets/img/output_5V_10uF_50V/probe_setup.jpg)

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | ![Waveform](assets/img/output_5V_10uF_50V/input_10V/DS2_QuickPrint129.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_10V/DS2_QuickPrint130.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_10V/DS2_QuickPrint131.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_10V/DS2_QuickPrint133.png) |
| 20V           | ![Waveform](assets/img/output_5V_10uF_50V/input_20V/DS2_QuickPrint134.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_20V/DS2_QuickPrint135.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_20V/DS2_QuickPrint136.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_20V/DS2_QuickPrint137.png) |
| 48V           | ![Waveform](assets/img/output_5V_10uF_50V/input_48V/DS2_QuickPrint138.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_48V/DS2_QuickPrint139.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_48V/DS2_QuickPrint140.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_48V/DS2_QuickPrint141.png) |

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | ![Waveform](assets/img/output_5V_10uF_50V/input_10V_noise/DS2_QuickPrint143.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_10V_noise/DS2_QuickPrint144.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_10V_noise/DS2_QuickPrint145.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_10V_noise/DS2_QuickPrint146.png) |
| 20V           | ![Waveform](assets/img/output_5V_10uF_50V/input_20V_noise/DS2_QuickPrint151.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_20V_noise/DS2_QuickPrint151.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_20V_noise/DS2_QuickPrint153.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_20V_noise/DS2_QuickPrint154.png) |
| 48V           | ![Waveform](assets/img/output_5V_10uF_50V/input_48V_noise/DS2_QuickPrint1.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_48V_noise/DS2_QuickPrint2.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_48V_noise/DS2_QuickPrint3.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_48V_noise/DS2_QuickPrint4.png) |

#### Noise

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | 73.60 mV (1.47%) | 73.60 mV (1.47%) | 20.80 mV (0.42%) | 19.20 mV (0.38%) |
| 20V           | 49.20 mV (0.98%) | 49.20 mV (0.98%) | 26.00 mV (0.52%) | 27.20 mV (0.54%) |
| 48V           | 49.20 mV (0.98%) | 49.20 mV (0.98%) | 45.20 mV (0.90%) | 40.40 mV (0.81%) |

### Output (5V, 2x 22uF 16V output capacitors)

![Probe Setup](assets/img/output_5V_22uF_16V/probe_setup.jpg)

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | ![Waveform](assets/img/output_5V_22uF_16V/input_10V/DS2_QuickPrint5.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_10V/DS2_QuickPrint6.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_10V/DS2_QuickPrint7.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_10V/DS2_QuickPrint8.png) |
| 20V           | ![Waveform](assets/img/output_5V_22uF_16V/input_20V/DS2_QuickPrint9.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_20V/DS2_QuickPrint10.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_20V/DS2_QuickPrint11.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_20V/DS2_QuickPrint12.png) |
| 48V           | ![Waveform](assets/img/output_5V_22uF_16V/input_48V/DS2_QuickPrint13.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_48V/DS2_QuickPrint14.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_48V/DS2_QuickPrint15.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_48V/DS2_QuickPrint16.png) |

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | ![Waveform](assets/img/output_5V_22uF_16V/input_10V_noise/DS2_QuickPrint17.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_10V_noise/DS2_QuickPrint18.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_10V_noise/DS2_QuickPrint19.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_10V_noise/DS2_QuickPrint20.png) |
| 20V           | ![Waveform](assets/img/output_5V_22uF_16V/input_20V_noise/DS2_QuickPrint25.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_20V_noise/DS2_QuickPrint26.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_20V_noise/DS2_QuickPrint27.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_20V_noise/DS2_QuickPrint28.png) |
| 48V           | ![Waveform](assets/img/output_5V_22uF_16V/input_48V_noise/DS2_QuickPrint29.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_48V_noise/DS2_QuickPrint30.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_48V_noise/DS2_QuickPrint31.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_48V_noise/DS2_QuickPrint32.png) |

#### Noise

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | 31.40 mV (0.63%) | 32.40 mV (0.65%) | 16.40 mV (0.33%) | 15.20 mV (0.30%) |
| 20V           | 22.80 mV (0.46%) | 24.40 mV (0.49%) | 19.60 mV (0.39%) | 19.20 mV (0.38%) |
| 48V           | 23.60 mV (0.47%) | 26.20 mV (0.52%) | 21.00 mV (0.42%) | 21.20 mV (0.42%) |

### Output (24V, 2x 10uF 50V output capacitors)

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | ![Waveform](assets/img/output_5V_10uF_50V/input_10V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_10V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_10V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_10V/DS2_QuickPrint.png) |
| 20V           | ![Waveform](assets/img/output_5V_10uF_50V/input_20V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_20V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_20V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_20V/DS2_QuickPrint.png) |
| 48V           | ![Waveform](assets/img/output_5V_10uF_50V/input_48V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_48V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_48V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_48V/DS2_QuickPrint.png) |

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | ![Waveform](assets/img/output_5V_10uF_50V/input_10V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_10V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_10V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_10V_noise/DS2_QuickPrint.png) |
| 20V           | ![Waveform](assets/img/output_5V_10uF_50V/input_20V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_20V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_20V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_20V_noise/DS2_QuickPrint.png) |
| 48V           | ![Waveform](assets/img/output_5V_10uF_50V/input_48V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_48V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_48V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_10uF_50V/input_48V_noise/DS2_QuickPrint.png) |

#### Noise

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           |  mV (%) |  mV (%) |  mV (%) |  mV (%) |
| 20V           |  mV (%) |  mV (%) |  mV (%) |  mV (%) |
| 48V           |  mV (%) |  mV (%) |  mV (%) |  mV (%) |


## PCB v1.0.0-5-g07f53f4 (hack1)

### Switching converter analysis (LMR51625)

![Overview](assets/img/hack1/sw_node_overview.jpg)

50 ohms series termination at the SW node.

![Closeup](assets/img/hack1/sw_node_closeup.jpg)

#### Switch node

| Input Voltage | Waveform | Rising edge |
|---------------|----------|-------------|
| 10V           | ![Waveform](assets/img/hack1/sw_node_10V_400mA/DS2_QuickPrint33.png) | ![Rising](assets/img/hack1/sw_node_10V_400mA/DS2_QuickPrint34.png) |
| 20V           | ![Waveform](assets/img/hack1/sw_node_20V_400mA/DS2_QuickPrint35.png) | ![Rising](assets/img/hack1/sw_node_20V_400mA/DS2_QuickPrint36.png) |
| 48V           | ![Waveform](assets/img/hack1/sw_node_48V_500mA/DS2_QuickPrint37.png) | ![Rising](assets/img/hack1/sw_node_48V_500mA/DS2_QuickPrint38.png) |

### Output (5V, LMR51625, 2x 22uF 16V output capacitors)

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | ![Waveform](assets/img/output_5V_22uF_16V/input_10V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_10V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_10V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_10V/DS2_QuickPrint.png) |
| 20V           | ![Waveform](assets/img/output_5V_22uF_16V/input_20V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_20V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_20V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_20V/DS2_QuickPrint.png) |
| 48V           | ![Waveform](assets/img/output_5V_22uF_16V/input_48V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_48V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_48V/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_48V/DS2_QuickPrint.png) |

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | ![Waveform](assets/img/output_5V_22uF_16V/input_10V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_10V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_10V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_10V_noise/DS2_QuickPrint.png) |
| 20V           | ![Waveform](assets/img/output_5V_22uF_16V/input_20V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_20V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_20V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_20V_noise/DS2_QuickPrint.png) |
| 48V           | ![Waveform](assets/img/output_5V_22uF_16V/input_48V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_48V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_48V_noise/DS2_QuickPrint.png) | ![Waveform](assets/img/output_5V_22uF_16V/input_48V_noise/DS2_QuickPrint.png) |

#### Noise

| Input Voltage | No Load | 50 mA | 500 mA | 1 A |
|---------------|---------|-------|--------|-----|
| 10V           | mV (%) | mV (%) | mV (%) | mV (%) |
| 20V           | mV (%) | mV (%) | mV (%) | mV (%) |
| 48V           | mV (%) | mV (%) | mV (%) | mV (%) |

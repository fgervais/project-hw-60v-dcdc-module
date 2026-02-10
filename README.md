# 4.3V to 60V input / 0.8V to 30V output switching converter

## Switch node analysis

![Overview](assets/img/sw_node_overview.jpg)

50 ohms series termination at the SW node.

![Closeup](assets/img/sw_node_closeup.jpg)

### Switch node

| Input Voltage | Waveform | Rising edge |
|---------------|----------|-------------|
| 10V           | ![Waveform](assets/img/sw_node_10V_400mA/DS2_QuickPrint96.png) | ![Rising](assets/img/sw_node_10V_400mA/DS2_QuickPrint97.png) |
| 20V           | ![Waveform](assets/img/sw_node_20V_400mA/DS2_QuickPrint98.png) | ![Rising](assets/img/sw_node_20V_400mA/DS2_QuickPrint99.png) |
| 48V           | ![Waveform](assets/img/sw_node_48V_500mA/DS2_QuickPrint100.png) | ![Rising](assets/img/sw_node_48V_500mA/DS2_QuickPrint102.png) |

## Output analysis

### Probe setup

<img src="assets/img/probe_overview.jpg" alt="probe overview"/>

Output capacitors -> 1uF capacitor -> 10 cm RG316 coax -> 50 ohms feed through termination

<img src="assets/img/probe_zoom.jpg" alt="probe zoom"/>

### 5V output / ~Max current

| Input voltage (V) | Current (A) | Temperature (°C)                                   | Noise (mVp-p) | Noise (%) | | |
|-------------------|-------------|----------------------------------------------------|---------------|-----------|-|-|
| 8                 | 2           | [59.8](assets/img/noise_5V/temperature_8V2A.jpg)   | 40            | 0.8       |![capture](assets/img/noise_5V/DS2_QuickPrint51.png)|![capture](assets/img/noise_5V/DS2_QuickPrint52.png)|
| 10                | 2           | [60.8](assets/img/noise_5V/temperature_10V2A.jpg)  | 42.4          | 0.848     |![capture](assets/img/noise_5V/DS2_QuickPrint53.png)|![capture](assets/img/noise_5V/DS2_QuickPrint54.png)|
| 20                | 1.5         | [62](assets/img/noise_5V/temperature_20V15A.jpg)   | 66.4          | 1.328     |![capture](assets/img/noise_5V/DS2_QuickPrint55.png)|![capture](assets/img/noise_5V/DS2_QuickPrint56.png)|
| 24                | 1.2         | [61.8](assets/img/noise_5V/temperature_24V12A.jpg) | 72.8          | 1.456     |![capture](assets/img/noise_5V/DS2_QuickPrint58.png)|![capture](assets/img/noise_5V/DS2_QuickPrint59.png)|
| 48                | 0.4         | [60.1](assets/img/noise_5V/temperature_48V04A.jpg) | 127.2         | 2.544     |![capture](assets/img/noise_5V/DS2_QuickPrint60.png)|![capture](assets/img/noise_5V/DS2_QuickPrint61.png)|

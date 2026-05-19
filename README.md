# BLDC Driver – STM32F405RGT6


基于 **STM32F405RGT6** 的高性能无刷直流电机（BLDC）驱动器，集成双路电压采集、CAN 总线接口、双路 SPI 绝对值编码器接口，支持 19V/20A 持续电流输出。适用于机器人关节、小型无人机电调、CNC 及 DIY 项目。

<img width="1015" height="498" alt="Snipaste_2026-05-19_17-20-32" src="https://github.com/user-attachments/assets/aed0012f-5f82-47be-bdce-928a489b9eb4" />


<img width="1060" height="562" alt="Snipaste_2026-05-19_17-20-41" src="https://github.com/user-attachments/assets/7c1378d8-fb78-4b2c-9e7b-e64e70ed63a4" />

---

## ✨ 特性

- **主控芯片**：STM32F405RGT6 (Cortex-M4，FPU，1MB Flash，192KB RAM)
- **供电电压**：12V–24V（标称 19V）
- **额定电流**：20A 持续（峰值 30A，<1s，需散热）
- **通信接口**：CAN 2.0A/B
- **编码器输入**：2× SPI 总线，MT6816 等spi编码器
- **PWM 驱动**：6 路互补 PWM（带死区插入）
- **电流采样**：2 路低侧电流采样接口
- **保护功能**：过流、过压、欠压、过热保护
- **调试接口**：SWD（4-pin） + 串口调试输出

---

## 📊 硬件规格

| 参数                | 值                          |
| ------------------- | --------------------------- |
| 输入电压            | 12 – 24 V DC （推荐 19 V）  |
| 持续电流            | 20 A （需散热片+风冷）      |
| 峰值电流（<1秒）    | 30 A                        |
| PWM 频率            | 8 kHz – 60 kHz（可编程）    |
| SPI 编码器频率      | 最高 10 MHz                 |
| CAN 速率            | 125k, 250k, 500k, 1M bps    |
| ADC 分辨率          | 12 位（0 – 30V 量程）       |
| 电压采样精度        | ±2%（经校准可达 ±1%）       |
| 工作温度            | -20°C ~ +60°C               |
| PCB 尺寸            | 78 mm × 35 mm               |

---


#### 克隆仓库

```bash
git clone https://github.com/yourname/bldc-driver-stm32f405.git
cd bldc-driver-stm32f405/Firmware

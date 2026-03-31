# Multi-Source Power Module.
📌 Project OverviewThis project features a high-efficiency power management board designed for robotics and embedded systems. It supports dual-input sources: Battery (Li-ion/LiPo) or a DC Wall Adapter, providing three stable output rails using a dedicated Buck-Boost architecture.
🚀 Key Features
- Dual Input: Flexible power from Battery or DC Jack.
- Triple Regulated Outputs: 12V, 5V, and 3.3V for various peripheral needs.
- High Current Capability: Designed to handle significant loads for motors and MCUs.
- Compact Design: Optimized PCB layout for minimal noise and heat dissipation.
🛠 Hardware Architecture & ComponentsThe board utilizes three specialized switching regulator stages to ensure maximum efficiency:
1. Boost Stage (12V Rail)
- IC: XL6019 (5A High-Current Boost DC-DC Converter)
- Purpose: Steps up the input voltage (from battery or adapter) to a stable 12V to power motors, fans, or high-power sensors.
3. Buck Stage (5V Rail)
- IC: TPS5430DDAR (3A, 500kHz Step-Down Converter)
- Purpose: Converts the 12V rail or input source down to 5V. Ideal for Arduino, ESP32, and standard 5V logic devices.
4. Buck Stage (3.3V Rail)
- IC: MP2307 (3A, 23V, 340kHz Synchronous Rectified Step-Down Converter)
- Purpose: Provides a high-precision 3.3V output for low-power MCUs (STM32), Wi-Fi modules, and modern digital sensors.
📊 Technical Specifications
Parameter                           Value
Input Voltage                [e.g., 5V - 15V DC]
Output 1 (XL6019)            12V @ Up to 2A (Continuous)
Output 2 (TPS5430)           5V @ Up to 3A
Output 3 (MP2307)            3.3V @ Up to 3A
Efficiency                   ~90% (depending on load)

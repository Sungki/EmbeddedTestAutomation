# Embedded Hardware-in-the-Loop (HIL) Test Automation PoC

This repository contains a production-ready **Proof of Concept (PoC)** demonstrating automated firmware validation and real-time hardware-level timing verification. It bridges physical test equipment and microcontrollers with cloud/local test execution.

## 🛠️ Key Architectural Highlights
*   **Instrument Automation**: Mimics controlling lab equipment (Oscilloscopes/Logic Analyzers via PyVISA commands).
*   **DUT Protocol Testing**: Simulates low-level serial (UART/SPI) byte injection and state validation to an STM32 MCU.
*   **Time-Constraint Assertions**: Evaluates hardware latency and execution jitter against strict real-time thresholds (e.g., electronic lock motor activation time).
*   **CI/CD Ready**: Structured to easily plug into PyTest frameworks under Azure DevOps or Jenkins pipelines.

## 🚀 How to Run Locally
1. Clone the repository:
   ```bash
   git clone
   pip install -r requirements.txt
   ```
2. Run the automation suite:
   ```bash
   python embedded_hil_test.py
   ```
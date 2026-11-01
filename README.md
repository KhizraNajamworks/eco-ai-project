# Eco AI Chatbot: Dynamic Power-Saving Assistant

An eco-conscious AI chatbot designed to minimize carbon footprints and electricity waste during inference. Instead of running heavy models for simple tasks, this chatbot dynamically chanages its processing power modes based on the complexity of the user's prompt. 

It also provides real-time hardware telemetry—like temperature, power draw, and response times—to give users complete visibility into their computing footprint.

---

##  Dynamic Intelligence Modes

To prevent unnecessary power and electricity consumption, the chatbot automatically switches between three distinct operational modes based on the weight of the question:

* **🟢 Easy Mode:** Triggered by light, simple questions. Uses minimal computing power and low electricity.
* **🟡 Eco Mode:** Triggered by standard, everyday queries. Balanced power distribution for efficient processing.
* **🔴 Full Mode:** Triggered by heavy requests (e.g., "explain in detail", complex logic, coding blocks). Unlocks maximum processing capability only when absolutely necessary.

---

## 📊 Real-Time Hardware Telemetry

Every time the AI generates a response, it outputs a performance dashboard showing exactly how it utilized the system's hardware:
* **Response Time:** How long the model took to process and answer.
* **System Temperature:** Monitors real-time hardware heat spikes during computation.
* **Active Mode:** Displays which power mode (Easy/Eco/Full) was engaged.
* **Power Efficiency Metrics:** Shows estimated energy saved by adjusting the model's footprint.

---
## 🛠️ Tech Stack & Requirements

* **Language:** Python 3
* **Local AI Engine:** [Ollama](https://ollama.com) (Runs open-source LLMs locally on-device)
* **GUI Framework:** `tkinter` (Built-in Python Graphical User Interface framework)
* **Hardware Integration:** Python runtime analysis, `time` metrics, and execution latency tracking.
* **Environment:** VS Code, Git, GitHub
  
---

##  How to Run Locally

1. Clone this repository to your computer.
2. Open your terminal inside this project folder.
3. Run the chatbot application:
   ```bash
   python eco_ai.py
   ```

---

## 📈 Future Roadmap
- [ ] Connect physical IoT hardware (like an external LED screen) to display temperature logs.
- [ ] Build a sleek frontend dashboard (using Streamlit or Tkinter) to graph power consumption over time.
- [ ] Integrate advanced token-length analysis for even more accurate mode switching.

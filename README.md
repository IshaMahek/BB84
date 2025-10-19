# 🔐 BB84 Quantum Key Distribution Protocol – Implementation using Qiskit

## 📘 Overview
This project implements the **BB84 Quantum Key Distribution (QKD)** protocol — the first and most widely studied method for secure quantum communication.  
Developed by **Charles Bennett and Gilles Brassard (1984)**, BB84 leverages the principles of **quantum mechanics**, such as superposition and measurement disturbance, to allow two parties (Alice and Bob) to establish a **shared secret key** securely, even in the presence of an eavesdropper (Eve).

This repository demonstrates the **quantum simulation** of BB84 using **Qiskit**, and includes a **basic Flask-based UI** to visualize the protocol flow and results.

---

## 🧠 Key Concepts
- **Qubits and Superposition:** Fundamental building blocks of quantum communication.
- **Polarization Bases:** Rectilinear (Z) and Diagonal (X) bases used for encoding bits.
- **No-Cloning Theorem:** Ensures eavesdroppers cannot copy unknown quantum states.
- **Error Estimation & Correction:** Detects and removes noise or interception effects.
- **Privacy Amplification:** Produces the final secure shared key.

---

## 🧩 Features
- Simulates **BB84 key exchange** between Alice and Bob using Qiskit.
- Implements **quantum encoding, transmission, measurement, and sifting**.
- Includes **error estimation and privacy amplification** logic.
- Basic **Flask UI** for user-friendly visualization of BB84 stages.
- Extensible design for future integration with real quantum devices or APIs.

---

## ⚙️ Tech Stack
| Component | Description |
|------------|--------------|
| **Python 3.x** | Core programming language |
| **Qiskit** | Quantum circuit design and simulation |
| **NumPy & Matplotlib** | Numerical operations and data visualization |
| **Flask** | Lightweight web framework for UI |
| **HTML & CSS** | Interface layout and styling |

---

## 🧪 Methodology
1. **Key Generation:**  
   Alice randomly generates bits and bases (Rectilinear or Diagonal).

2. **Quantum Encoding:**  
   Each bit is encoded into a qubit state according to its chosen basis.

3. **Transmission & Measurement:**  
   Qubits are sent to Bob; he measures each using random bases.

4. **Sifting:**  
   Alice and Bob keep only bits where their bases match.

5. **Error Estimation & Correction:**  
   A subset of bits is compared publicly to estimate the Quantum Bit Error Rate (QBER).

6. **Privacy Amplification:**  
   The sifted key is compressed to remove any potential eavesdropper knowledge.

---

## 💻 Installation & Setup

### Prerequisites
- Python ≥ 3.8  
- pip (Python package manager)

### Steps
```bash
# Clone the repository
git clone https://github.com/IshaMahek/BB84-QKD.git
cd BB84-QKD

# Install dependencies
pip install -r requirements.txt

# Run the Flask app
python app.py

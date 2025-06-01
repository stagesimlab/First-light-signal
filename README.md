# Safe Multi-Stage Loader Simulation

## 🎯 Purpose

This project simulates a multi-stage malware execution chain **for educational and red team training purposes only**. It is designed to demonstrate common evasion and execution tactics without executing any real malicious payloads.

## ✅ Safety First

This script:
- Does **not** connect to the network
- Does **not** execute any harmful payloads
- Uses `SAFETY_MODE = True` to disable potentially confusing behavior
- Is suitable for blue team exercises, workshops, and security education

## 🔍 Stages Simulated

| Stage | Name     | Description |
|-------|----------|-------------|
| 1     | Init     | Decodes and runs a mock staging module |
| 2     | Check    | Looks for signs of a sandbox/VM/analysis environment |
| 3     | Sleep    | Simulates delay and user activity |
| 4     | Decode   | AES-decrypts a mock payload in memory only |
| 5     | Execute  | Simulates execution (prints only) |
| 6     | Cleanup  | Overwrites and deletes dummy buffer |

## 🧪 How to Run

```bash
python safe_multistage_loader_demo.py
```

Make sure dependencies are installed:
```bash
pip install pycryptodome
```

## 📜 License

MIT License — or **"For Educational Use Only"** if you prefer.

---

### Red Team Labs  
This tool is designed to support safe simulation and detection of malware-like behavior without any malicious impact.

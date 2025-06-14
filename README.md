# 🌍 DERMS – Dispatcher System Simulation for Monitoring Distributed Energy Resource Production

## 📌 General Information
**Project Name:** Dispatcher System Simulation for Monitoring Distributed Energy Resource Production (DERMS)
**Goal:** Development of a simulation system that models a Smart Grid environment in which distributed generators (solar, wind) produce electrical energy and communicate with a central dispatcher server.

---

## 📝 Summary
The system simulates the operation of **prosumers** (producer-consumers) and includes:
- **Sensors** – generate weather condition data (solar irradiance, wind speed).
- **DER generators (clients)** – calculate energy production based on received data.
- **Dispatcher server** – centrally collects and processes production data, sends control messages, responds to unexpected values, and manages DER operations.

---

## ⚙️ Technical Description
- **Communication**
  - **TCP** – between sensors and DERs (transmitting weather conditions), between DERs and the dispatcher (sending calculated production).
  - **UDP** – between the dispatcher and DERs (on/off control messages).

- **Weather Condition Simulation**
  - **Solar panel:** generates solar irradiance (INS) and cell temperature (Tcell).
  - **Wind turbine:** generates random wind speed (0–30 m/s).

- **Security**
  - basic encryption of dispatcher commands

---
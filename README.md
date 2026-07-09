# 🛏️ SoftCare Sleep — Flexible Wearable Sleep Health Monitoring System

## 📌 Project Overview

**SoftCare Sleep** is a garment-integrated, flexible, and unobtrusive sleep health monitoring system. It embeds multi-site motion sensors, dual-channel temperature sensors, and photoelectric SpO₂/heart rate acquisition units into everyday sleepwear using flexible fabrication techniques, enabling **unrestricted, non-intrusive** sleep data collection. The system supports **head, torso, and arm** movement recognition with 5-level intensity grading, accurately identifying sleep events such as body turns, head rotations, and large arm movements. It features dual-channel temperature monitoring with sustained anomaly alerts and can detect blanket removal via temperature differential patterns. Continuous overnight SpO₂ and heart rate monitoring captures physiological fluctuations during sleep. Paired with a local PC-based analysis software, the system performs multi-source data fusion to generate structured sleep quality reports with quantitative scoring and personalized improvement recommendations. The entire workflow runs **offline locally**, ensuring data privacy and security without requiring internet connectivity.

---

## 🎯 Core Functions

- **Full-body Motion Monitoring**: 3-channel 9-axis IMU sensors with 5-level activity intensity grading, accurately identifying body turns, head rotations, and large arm movements.
- **Dual-channel Temperature Alerting**: Simultaneous monitoring of in-blanket body surface temperature and ambient temperature. Identifies blanket removal via temperature differential patterns, with automatic alerts triggered after 120 seconds of sustained anomalies.
- **Vital Signs Acquisition**: Photoplethysmographic (PPG) SpO₂ and heart rate sensors for continuous overnight monitoring, reflecting physiological fluctuations during sleep.
- **Intelligent Sleep Report**: Multi-dimensional weighted scoring model generating comprehensive sleep scores, sub-item analysis, and personalized health recommendations.
- **Flexible Unobtrusive Wear**: FPC flexible circuits embedded into fabric, ultra-thin with no protrusions, ensuring zero interference with natural sleep and compatibility with daily wear habits.

---

## 🏥 Application Scenarios

| Scenario | Value Proposition |
|----------|-------------------|
| **Home Health Management** | Daily sleep self-assessment for all age groups, promoting regular sleep routines |
| **Community Sleep Screening** | Low-cost screening tool for identifying high-risk individuals with sleep apnea and chronic insomnia |
| **Elderly Care Facility Monitoring** | Overnight long-term surveillance, detecting abnormal movements and prolonged blanket removal to reduce nocturnal incidents |
| **Post-surgery Rehabilitation Tracking** | Non-invasive sleep monitoring to assist recovery assessment and rehabilitation plan adjustments |

---

## ⚙️ Technical Features

- **Flexible Fabric Integration**: Ultra-thin FPC + miniaturized sensors, fully embedded into sleepwear for genuine unobtrusive wear.
- **Multi-modal Synchronous Acquisition**: IMU motion, dual-temperature, SpO₂/heart rate, and ECG data fusion, overcoming the limitations of single-dimensional assessments.
- **Intelligent Assessment Model**: Weighted fusion algorithm automatically generates quantitative scores and structured conclusions, forming a closed-loop from acquisition to analysis to evaluation.
- **Fully Offline Architecture**: Embedded real-time acquisition + PC-based local analysis. No network required; all data stored locally to guarantee privacy.

---

## 📊 Key Performance Specifications

| Module | Key Specifications |
|--------|-------------------|
| **SpO₂ / Heart Rate** | Sampling rate 200Hz; HR range 40–180 bpm; SpO₂ threshold ≥94%; Signal quality 0–100 |
| **Motion/Posture** | 3-channel 9-axis sync; 5-level grading thresholds (3°/6°/10°/20°); turn detection at cumulative 30° |
| **Temperature** | Dual-channel sync; ΔT < 2°C for 5 min identifies blanket removal; alert after 120s anomaly |
| **Sleep Scoring** | Total 0–100; Motion 60% + Vitals 30% + Stability 10%; Five-tier grading |
| **Communication/UI** | Bluetooth baud rate 921600; UI refresh 20ms; Supports 30s waveform review; JSON report export |

---

## 💡 Innovation Highlights

1. **Genuinely Unobtrusive Wear**: Replaces rigid enclosures with flexible fabric integration, providing a comfortable platform for long-term home-based monitoring.
2. **Comprehensive Multi-dimensional Monitoring**: Integrates motion, temperature, SpO₂, heart rate, and ECG to fully reconstruct overnight sleep status.
3. **Intelligent Assessment Closed-loop**: Transforms raw data into quantitative scores and structured recommendations, making monitoring results truly actionable for health management.

---

## 🧩 System Architecture

Three-tier collaborative architecture:

- **Perception Layer**: Dual-temperature, IMU motion, SpO₂/heart rate, and ECG modules for synchronized multi-source acquisition.
- **Terminal Processing Layer**: Lithium battery powered; main controller receives and preprocesses data; transmits to host via Bluetooth.
- **Local Analysis Layer**: Data reception, fusion, statistical analysis, sleep scoring, and report generation—all completed locally.

---

## 🧪 Completion Status & Achievements

- ✅ Full system prototype developed, including flexible sensor-integrated garment, main control board, charging accessories, and complete software suite.
- ✅ Flexible garment sample validated: withstands bending and stretching without circuit fractures; comfortable to wear and machine-washable (with control board removed).
- ✅ High-density 4-layer PCB main control board with stable module performance, supporting continuous overnight monitoring.
- ✅ Full-stack software (embedded + PC) integrated and validated. Clear graphical interface with intuitive operation.

---

## 📈 Validated Performance

- **Motion Detection**: Reliably identifies 3-site independent movements with 5-level intensity grading; accurately marks body turns, head rotations, and arm movements with precise timestamps.
- **Temperature Monitoring**: Dual-channel differential reliably detects blanket removal; threshold alerts respond accurately.
- **SpO₂ / Heart Rate**: 200Hz sampling with 0.7–4Hz bandpass filtering; automatic anomaly tagging; vital signs dimension incorporated into scoring.
- **Report Generation**: One-click generation of structured reports covering composite score, motion analysis, vital signs, temperature comfort assessment, and health recommendations.

---

## 🔮 Future Extensions

- **Expanded Monitoring Dimensions**: Enhance EMG, ECG, and respiratory rate analysis, progressively approaching clinical-grade screening standards.
- **On-device Intelligence**: Deploy lightweight algorithms for local real-time alerts on sleep apnea, nocturnal tremors, and other risk events.
- **Ecosystem Integration**: Develop smart home connectivity protocols to automatically adjust ambient temperature, lighting, etc., based on sleep stages—creating a "monitoring-intervention" closed loop.
- **Form Factor Optimization**: Develop multiple styles and sizes; further miniaturize control board and extend battery life.

---

## 🙌 Project Reflections

From concept to physical prototype, we have come to deeply appreciate that **product development is about finding optimal solutions within real-world constraints—cost, size, power consumption, and user experience**. Every detail in hardware design was iterated repeatedly; algorithms evolved from complexity to lightweight practicality. Ultimately, we delivered a stable, user-friendly, and genuinely valuable sleep monitoring solution. We will continue to refine "SoftCare Sleep" to make it even more complete and accessible to those who need it.

---

> 📅 Project Status: Prototype completed and functionally validated. Continuous iteration and optimization in progress.

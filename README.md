# Lacco FHIR Profiles

## 🎬 Pitch Video

▶️ **[Watch on Vimeo](https://vimeo.com/1154677257)** - 5-minute pitch for Finnish Health Data Hackathon 2026

*Alternative: [Download from GitHub](./pitch-video.mp4) (13 MB)*

---

FHIR Implementation Guide for environmental-physiological monitoring in CPAP therapy optimization and asthma management.

**Developed at:** Finnish Health Data Hackathon 2026  
**Track:** Care Plans and Clinical Reasoning  
**Developer:** Arto Kivimäki  
**Contact:** arto.kivimaki@tutanota.com  
**Status:** Work in progress

## Overview

Lacco is a wearable multisensor device that simultaneously measures:
- Environmental: CO₂, VOC, temperature, humidity, UV
- Physiological: SpO₂, HRV, GSR, respiration, body temperature

**Primary use:** CPAP therapy optimization for sleep apnea  
**Secondary use:** Asthma environmental trigger identification

## Clinical Problem

CPAP devices measure only pressure and airflow, not environmental factors. 
Patients experience poor sleep despite correct CPAP settings because:
- High bedroom CO₂ (>1600 ppm) causes central sleep apnea
- Poor air quality (VOC) causes arousals
- Current systems cannot distinguish CPAP issues from environmental issues

## Lacco Solution

First device combining environmental and physiological monitoring for CPAP optimization.

## Repository Structure

- `profiles/` - FHIR StructureDefinition profiles
- `examples/` - Example FHIR instances
- `cds-hooks/` - CDS Hooks service definitions
- `docs/` - Documentation and implementation guide

## Profiles

- **LaccoCO2Observation** - Indoor CO₂ concentration
- **LaccoVOCObservation** - Volatile organic compounds
- **LaccoDevice** - Multisensor wearable device
- **CPAPCarePlan** - CPAP therapy with environmental monitoring

## CDS Hooks

- **cpap-suboptimal-environment** - Alert when high CO₂ affects CPAP therapy

## License

### Software and FHIR Profiles

This project's **FHIR profiles, example data, CDS Hooks, and software code** are licensed under the **MIT License**.

You are free to:
- ✅ Use, modify, and distribute the FHIR profiles
- ✅ Integrate them into commercial or non-commercial projects
- ✅ Fork and adapt for your own use cases

See [LICENSE](LICENSE) for full details.

### Device Concept

The underlying **wearable device concept** (simultaneous physiological and environmental monitoring) is subject to:

**Finnish Utility Model Application**  
Filed: December 8, 2025  
Status: Pending examination

**Important:**
- The MIT License covers **only the software and data models** in this repository
- It does **NOT grant rights** to manufacture, distribute, or commercialize devices based on the utility model
- The device concept remains subject to intellectual property protection

For device licensing inquiries or research collaboration on the hardware concept, contact: [arto.kivimaki@tutanota.com](mailto:arto.kivimaki@tutanota.com)

## Contact

Arto Kivimäki | arto.kivimaki@tutanota.com  
GitHub: https://github.com/ArtOfSensorTech/lacco-fhir-profiles

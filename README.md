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

MIT License

## Contact

Arto Kivimäki | arto.kivimaki@tutanota.com  
GitHub: https://github.com/ArtOfSensorTech/lacco-fhir-profiles

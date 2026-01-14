# Lacco - Hackathon Pitch

**Finnish Health Data Hackathon 2026**  
**Track:** Care Plans and Clinical Reasoning  
**Developer:** Arto Kivimäki (Remote from Romania)

## Problem: CPAP Therapy Doesn't Always Work

CPAP devices measure only pressure and airflow, not environmental factors.

**Patient scenario:**
- CPAP pressure: ✅ Correct (12 cmH₂O)
- CPAP adherence: ✅ Good (7.5 hours/night)
- Sleep quality: ❌ Poor (frequent awakenings)

**Why?** Current systems cannot answer: Is it CPAP settings or bedroom environment?

## Solution: Lacco Device

Wearable multisensor measuring simultaneously:
- Environmental: CO₂, VOC, temperature, humidity
- Physiological: SpO₂, HRV, respiration

**Key Innovation:** Same device = timestamp-synchronized measurements

## Example Case

**Night monitoring:**
- CPAP: 12 cmH₂O, 7.5h use ✅
- Bedroom CO₂: 2100 ppm ⚠️ (very high)
- HRV: 45 ms (low - indicates stress)

**Diagnosis:** Environment problem, not CPAP  
**Action:** Improve ventilation, don't adjust CPAP

## Hackathon Goals

1. FHIR CarePlan profile for CPAP + environmental monitoring
2. Observation profiles: CO₂, VOC, HRV
3. CDS Hooks: "cpap-suboptimal-environment"
4. Device integration model
5. Public examples for FHIR community

## Contact

Arto Kivimäki | arto.kivimaki@tutanota.com  
GitHub: https://github.com/ArtOfSensorTech/lacco-fhir-profiles

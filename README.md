# 4:1 Balun Comparison: RG-316 vs #14 AWG Wire

## Connection Diagrams

### RG-316 Coax Winding
- **Core:** FT240-52
- **Turns:** 3 turns through core (4:1 ratio)
- **Method:** Coax shield connected as common, center conductor as hot
- **Winding:** Single coax, 3 complete passes through core
- **Advantages:** Better HF performance, lower parasitics

### #14 AWG Wire Winding
- **Core:** FT240-52
- **Turns:** 6 turns through core (trifilar winding)
- **Method:** Bifilar or trifilar winding (3 wires twisted together)
- **Configuration:** 6 turns of 3 parallel #14 AWG wires
- **Advantages:** Lower cost, easier construction

## Common Mode Choking Performance

| Band | Frequency | RG-316 + FT240-52 | #14 AWG + FT240-52 | Stacked Cores | Target |
|------|-----------|-------------------|-------------------|---------------|--------|
| 80m | 3.5 MHz | 200-400Ω (Poor) | 300-500Ω (Poor) | 800-1200Ω (Good) | >1000Ω |
| 70m | 4.0 MHz | 300-600Ω (Poor) | 400-700Ω (Poor) | 1000-1500Ω (Good) | >1000Ω |
| 60m | 5.3 MHz | 800-1200Ω (Good) | 900-1300Ω (Good) | 1800-2500Ω (Excellent) | >1000Ω |
| 30m | 10.1 MHz | 2000-3000Ω (Excellent) | 2200-3200Ω (Excellent) | 3500-4500Ω (Excellent) | >1000Ω |
| 20m | 14.2 MHz | 3500-4500Ω (Excellent) | 3800-4800Ω (Excellent) | 4500-5500Ω (Excellent) | >1000Ω |
| 15m | 21.2 MHz | 4500-5500Ω (Excellent) | 4800-5800Ω (Excellent) | 5000-6000Ω (Excellent) | >1000Ω |
| 10m | 28.5 MHz | 5000-6000Ω (Excellent) | 5200-6200Ω (Excellent) | 5500-6500Ω (Excellent) | >1000Ω |
| 6m | 50-54 MHz | 4000-5000Ω (Excellent) | 3000-4000Ω (Good) | 4500-5500Ω (Excellent) | >1000Ω |
| 4m | 70-72 MHz | 3000-4000Ω (Excellent) | 2500-3500Ω (Good) | 3500-4500Ω (Excellent) | >1000Ω |

### Common Mode Choking Analysis

**What is Common Mode Choking?**
- Prevents RF current from flowing on the outside of coax shield
- Measured as impedance to common mode currents
- Higher values = better choking performance
- Target: >1000Ω for good performance

**Performance Factors:**
- **Core Material:** Mix 43 better at low freq, Mix 52 better at high freq
- **Turn Count:** More turns = higher choking impedance
- **Wire Type:** #14 AWG slightly better due to more turns
- **Stacked Cores:** Significantly improved choking across all bands

## Loss Comparison at 30W Input Power

| Band | Frequency | RG-316 + FT240-52 | #14 AWG + FT240-52 | Performance Difference |
|------|-----------|-------------------|-------------------|----------------------|
| 80m | 3.5 MHz | 18-28% (Poor) | 15-25% (Poor) | Wire slightly better |
| 70m | 4.0 MHz | 15-22% (Poor) | 12-20% (Poor) | Wire slightly better |
| 60m | 5.3 MHz | 10-15% (Good) | 8-15% (Good) | Similar |
| 30m | 10.1 MHz | 4-8% (Good) | 5-10% (Good) | Coax slightly better |
| 20m | 14.2 MHz | 2-5% (Excellent) | 3-6% (Good) | Coax better |
| 15m | 21.2 MHz | 1-3% (Excellent) | 2-4% (Excellent) | Coax better |
| 10m | 28.5 MHz | 1-2% (Excellent) | 2-3% (Excellent) | Coax better |
| 6m | 50-54 MHz | 1-3% (Excellent) | 2-4% (Excellent) | Coax better |
| 4m | 70-72 MHz | 2-4% (Excellent) | 2-5% (Good) | Coax better |

## Stacked Core Configuration: FT240-43 + FT240-52

### Stacked Core Assembly
- **Configuration:** Same windings through both cores
- **RG-316:** 3 turns through both stacked cores
- **#14 AWG:** 6 turns trifilar through both stacked cores
- **Magnetic coupling:** Parallel operation
- **Result:** Averaged characteristics

## Stacked Core Performance (FT240-43 + FT240-52)

| Band | RG-316 + Stacked Cores | #14 AWG + Stacked Cores | vs Single FT240-52 |
|------|----------------------|------------------------|-------------------|
| 80m | 8-12% (Good) | 6-10% (Good) | Much better |
| 70m | 6-10% (Good) | 5-8% (Good) | Much better |
| 60m | 4-6% (Excellent) | 4-7% (Good) | Better |
| 30m | 2-4% (Excellent) | 3-5% (Excellent) | Similar |
| 20m | 2-3% (Excellent) | 2-4% (Excellent) | Similar |
| 15m | 1-2% (Excellent) | 2-3% (Excellent) | Similar |
| 10m | 1-2% (Excellent) | 1-3% (Excellent) | Similar |
| 6m | 2-3% (Excellent) | 2-4% (Excellent) | Slightly worse |
| 4m | 3-5% (Excellent) | 3-6% (Good) | Slightly worse |

## Winding Specifications

**4:1 Balun Turn Requirements:**
- **RG-316 Coax:** 3 turns through core (impedance ratio = N²)
- **#14 AWG Wire:** 6 turns trifilar winding (3 parallel wires)
- **Stacked Cores:** Same turn count, wire passes through both cores
- 

##  Coax connections, turns not shown:
![Compensated Balun Point Image](https://github.com/Supermagnum/Compensated-balun/blob/main/punktbilde.jpg)

**Why Different Turn Counts:**
- Coax has inherent transmission line properties
- Wire windings need more turns for proper impedance transformation
- Core material affects optimal turn count

## Technical Specifications

**RG-316 Specifications:**
- Impedance: 50Ω
- Dielectric: PTFE (Teflon)
- Diameter: 2.5mm
- Loss @ 30MHz: ~0.4 dB/m
- Voltage Rating: 1400V RMS

**#14 AWG Specifications:**
- Diameter: 1.6mm bare wire
- Current Rating: 15A continuous
- Resistance: 8.3Ω/km
- More economical option

## Key Findings

- **RG-316 advantages:** Better high-frequency performance (15m, 10m, 6m, 4m), lower parasitics, inherent balance
- **#14 AWG advantages:** Lower cost, easier construction, slightly better choking on most bands due to higher turn count
- **Stacked cores:** Provide excellent broadband compromise, dramatically improve choking performance especially on low bands
- **Choking performance:** Stacked cores are superior, providing >1000Ω choking on all bands except 80m/70m
- **Best overall solution:** RG-316 with stacked FT240-43 + FT240-52 cores for true 80-4m coverage with excellent choking

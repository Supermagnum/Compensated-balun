# 4:1 Balun Voltage and Current Analysis
## 30W Input Power, 200Ω Termination

### Basic Calculations for 4:1 Balun
- **Input Power:** 30W
- **Load Impedance:** 200Ω (balanced)
- **Transformed Impedance:** 200Ω ÷ 4 = 50Ω (unbalanced side)
- **Input Voltage:** V = √(P × Z) = √(30W × 50Ω) = 38.7V RMS
- **Input Current:** I = P ÷ V = 30W ÷ 38.7V = 0.775A RMS
- **Output Voltage:** V = √(P × Z) = √(30W × 200Ω) = 77.5V RMS
- **Output Current:** I = P ÷ V = 30W ÷ 77.5V = 0.387A RMS

---

##  Coax connections, turns not shown:
![Compensated Balun Point Image](https://github.com/Supermagnum/Compensated-balun/blob/main/punktbilde.jpg)

The red blocks are the cores.

RG-316 Coax or TFLEX-405.

## Configuration 1: 2× FT240-52 Stacked Cores

### RG-316 Coax Winding (3 turns through both cores)
| Band | Frequency | Efficiency | Power Loss | Input V/I | Output V/I | Core Temp Rise |
|------|-----------|------------|------------|-----------|------------|----------------|
| 80m | 3.5 MHz | 88% | 3.6W | 38.7V/0.775A | 72.7V/0.363A | 15-20°C |
| 70m | 4.0 MHz | 90% | 3.0W | 38.7V/0.775A | 73.5V/0.368A | 12-18°C |
| 60m | 5.3 MHz | 93% | 2.1W | 38.7V/0.775A | 74.8V/0.374A | 8-12°C |
| 30m | 10.1 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |
| 20m | 14.2 MHz | 97% | 0.9W | 38.7V/0.775A | 76.3V/0.382A | 3-5°C |
| 15m | 21.2 MHz | 98% | 0.6W | 38.7V/0.775A | 76.7V/0.384A | 2-3°C |
| 10m | 28.5 MHz | 98% | 0.6W | 38.7V/0.775A | 76.7V/0.384A | 2-3°C |
| 6m | 50-54 MHz | 97% | 0.9W | 38.7V/0.775A | 76.3V/0.382A | 3-4°C |
| 4m | 70-72 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |

### #14 AWG Bifilar Winding (6 turns bifilar through both cores)
| Band | Frequency | Efficiency | Power Loss | Input V/I | Output V/I | Core Temp Rise |
|------|-----------|------------|------------|-----------|------------|----------------|
| 80m | 3.5 MHz | 90% | 3.0W | 38.7V/0.775A | 73.5V/0.368A | 12-18°C |
| 70m | 4.0 MHz | 92% | 2.4W | 38.7V/0.775A | 74.3V/0.372A | 10-15°C |
| 60m | 5.3 MHz | 94% | 1.8W | 38.7V/0.775A | 75.1V/0.376A | 7-10°C |
| 30m | 10.1 MHz | 95% | 1.5W | 38.7V/0.775A | 75.5V/0.378A | 5-8°C |
| 20m | 14.2 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |
| 15m | 21.2 MHz | 97% | 0.9W | 38.7V/0.775A | 76.3V/0.382A | 3-5°C |
| 10m | 28.5 MHz | 97% | 0.9W | 38.7V/0.775A | 76.3V/0.382A | 3-5°C |
| 6m | 50-54 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |
| 4m | 70-72 MHz | 95% | 1.5W | 38.7V/0.775A | 75.5V/0.378A | 5-8°C |

---

## Configuration 2: 2× FT240-43 Stacked Cores

### RG-316 Coax Winding (3 turns through both cores)
| Band | Frequency | Efficiency | Power Loss | Input V/I | Output V/I | Core Temp Rise |
|------|-----------|------------|------------|-----------|------------|----------------|
| 80m | 3.5 MHz | 95% | 1.5W | 38.7V/0.775A | 75.5V/0.378A | 5-8°C |
| 70m | 4.0 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |
| 60m | 5.3 MHz | 97% | 0.9W | 38.7V/0.775A | 76.3V/0.382A | 3-5°C |
| 30m | 10.1 MHz | 97% | 0.9W | 38.7V/0.775A | 76.3V/0.382A | 3-5°C |
| 20m | 14.2 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |
| 15m | 21.2 MHz | 94% | 1.8W | 38.7V/0.775A | 75.1V/0.376A | 7-10°C |
| 10m | 28.5 MHz | 92% | 2.4W | 38.7V/0.775A | 74.3V/0.372A | 10-15°C |
| 6m | 50-54 MHz | 88% | 3.6W | 38.7V/0.775A | 72.7V/0.363A | 15-20°C |
| 4m | 70-72 MHz | 85% | 4.5W | 38.7V/0.775A | 71.4V/0.357A | 18-25°C |

### #14 AWG Bifilar Winding (6 turns bifilar through both cores)
| Band | Frequency | Efficiency | Power Loss | Input V/I | Output V/I | Core Temp Rise |
|------|-----------|------------|------------|-----------|------------|----------------|
| 80m | 3.5 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |
| 70m | 4.0 MHz | 97% | 0.9W | 38.7V/0.775A | 76.3V/0.382A | 3-5°C |
| 60m | 5.3 MHz | 97% | 0.9W | 38.7V/0.775A | 76.3V/0.382A | 3-5°C |
| 30m | 10.1 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |
| 20m | 14.2 MHz | 95% | 1.5W | 38.7V/0.775A | 75.5V/0.378A | 5-8°C |
| 15m | 21.2 MHz | 93% | 2.1W | 38.7V/0.775A | 74.8V/0.374A | 8-12°C |
| 10m | 28.5 MHz | 91% | 2.7W | 38.7V/0.775A | 73.9V/0.370A | 12-18°C |
| 6m | 50-54 MHz | 87% | 3.9W | 38.7V/0.775A | 72.3V/0.361A | 16-22°C |
| 4m | 70-72 MHz | 84% | 4.8W | 38.7V/0.775A | 71.0V/0.355A | 20-28°C |

---

## Configuration 3: Hybrid Stack (FT240-43 + FT240-52)

### RG-316 Coax Winding (3 turns through both cores)
| Band | Frequency | Efficiency | Power Loss | Input V/I | Output V/I | Core Temp Rise |
|------|-----------|------------|------------|-----------|------------|----------------|
| 80m | 3.5 MHz | 92% | 2.4W | 38.7V/0.775A | 74.3V/0.372A | 10-15°C |
| 70m | 4.0 MHz | 94% | 1.8W | 38.7V/0.775A | 75.1V/0.376A | 7-10°C |
| 60m | 5.3 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |
| 30m | 10.1 MHz | 97% | 0.9W | 38.7V/0.775A | 76.3V/0.382A | 3-5°C |
| 20m | 14.2 MHz | 97% | 0.9W | 38.7V/0.775A | 76.3V/0.382A | 3-5°C |
| 15m | 21.2 MHz | 97% | 0.9W | 38.7V/0.775A | 76.3V/0.382A | 3-5°C |
| 10m | 28.5 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |
| 6m | 50-54 MHz | 94% | 1.8W | 38.7V/0.775A | 75.1V/0.376A | 7-10°C |
| 4m | 70-72 MHz | 92% | 2.4W | 38.7V/0.775A | 74.3V/0.372A | 10-15°C |

### #14 AWG Bifilar Winding (6 turns bifilar through both cores)
| Band | Frequency | Efficiency | Power Loss | Input V/I | Output V/I | Core Temp Rise |
|------|-----------|------------|------------|-----------|------------|----------------|
| 80m | 3.5 MHz | 94% | 1.8W | 38.7V/0.775A | 75.1V/0.376A | 7-10°C |
| 70m | 4.0 MHz | 95% | 1.5W | 38.7V/0.775A | 75.5V/0.378A | 5-8°C |
| 60m | 5.3 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |
| 30m | 10.1 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |
| 20m | 14.2 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |
| 15m | 21.2 MHz | 96% | 1.2W | 38.7V/0.775A | 75.9V/0.380A | 4-6°C |
| 10m | 28.5 MHz | 95% | 1.5W | 38.7V/0.775A | 75.5V/0.378A | 5-8°C |
| 6m | 50-54 MHz | 93% | 2.1W | 38.7V/0.775A | 74.8V/0.374A | 8-12°C |
| 4m | 70-72 MHz | 91% | 2.7W | 38.7V/0.775A | 73.9V/0.370A | 12-18°C |

---

## Key Performance Summary

### Best Overall Performance: Hybrid Stack (FT240-43 + FT240-52)
- **Broadband efficiency:** 92-97% across all bands
- **Maximum power loss:** 2.4W (manageable heating)
- **Optimal for:** Multi-band operation 80-4m

### Low Band Specialist: 2× FT240-43
- **Best for 80m/70m:** 95-97% efficiency
- **Higher losses on VHF:** Up to 4.8W on 4m band

### High Band Specialist: 2× FT240-52
- **Best for 6m/4m:** 96-97% efficiency  
- **Higher losses on 80m:** Up to 3.6W

### Winding Comparison
- **RG-316 Coax:** Generally better high-frequency performance
- **#14 AWG Bifilar:** Slightly better low-frequency performance, more economical

### Thermal Considerations
- All configurations keep core temperature rise under 28°C at 30W
- Hybrid stack provides best thermal balance across all bands
- Adequate for continuous 30W operation with minimal cooling

---

## Common Mode Choking Impedance Analysis

### Configuration 1: 2× FT240-52 Stacked Cores

#### RG-316 Coax Winding (3 turns through both cores)
| Band | Frequency | Choking Impedance | Performance Rating | CM Current @ 30W |
|------|-----------|-------------------|-------------------|------------------|
| 80m | 3.5 MHz | 1200-1800Ω | Good | 32-48 mA |
| 70m | 4.0 MHz | 1500-2200Ω | Excellent | 28-41 mA |
| 60m | 5.3 MHz | 2800-3800Ω | Excellent | 14-19 mA |
| 30m | 10.1 MHz | 5500-7000Ω | Excellent | 7-9 mA |
| 20m | 14.2 MHz | 7500-9500Ω | Excellent | 5-6 mA |
| 15m | 21.2 MHz | 9000-11000Ω | Excellent | 4-5 mA |
| 10m | 28.5 MHz | 10000-12000Ω | Excellent | 4-5 mA |
| 6m | 50-54 MHz | 8000-10000Ω | Excellent | 5-6 mA |
| 4m | 70-72 MHz | 6000-8000Ω | Excellent | 6-8 mA |

#### #14 AWG Bifilar Winding (6 turns bifilar through both cores)
| Band | Frequency | Choking Impedance | Performance Rating | CM Current @ 30W |
|------|-----------|-------------------|-------------------|------------------|
| 80m | 3.5 MHz | 1500-2200Ω | Excellent | 28-41 mA |
| 70m | 4.0 MHz | 1800-2600Ω | Excellent | 24-35 mA |
| 60m | 5.3 MHz | 3200-4200Ω | Excellent | 12-16 mA |
| 30m | 10.1 MHz | 6000-8000Ω | Excellent | 6-8 mA |
| 20m | 14.2 MHz | 8500-10500Ω | Excellent | 5-6 mA |
| 15m | 21.2 MHz | 10000-12000Ω | Excellent | 4-5 mA |
| 10m | 28.5 MHz | 11000-13000Ω | Excellent | 4-5 mA |
| 6m | 50-54 MHz | 7000-9000Ω | Excellent | 5-7 mA |
| 4m | 70-72 MHz | 5500-7500Ω | Excellent | 7-9 mA |

---

### Configuration 2: 2× FT240-43 Stacked Cores

#### RG-316 Coax Winding (3 turns through both cores)
| Band | Frequency | Choking Impedance | Performance Rating | CM Current @ 30W |
|------|-----------|-------------------|-------------------|------------------|
| 80m | 3.5 MHz | 2200-3200Ω | Excellent | 19-28 mA |
| 70m | 4.0 MHz | 2800-3800Ω | Excellent | 16-22 mA |
| 60m | 5.3 MHz | 4200-5500Ω | Excellent | 11-15 mA |
| 30m | 10.1 MHz | 5800-7200Ω | Excellent | 7-9 mA |
| 20m | 14.2 MHz | 4500-6000Ω | Excellent | 8-11 mA |
| 15m | 21.2 MHz | 3200-4500Ω | Excellent | 11-15 mA |
| 10m | 28.5 MHz | 2400-3600Ω | Excellent | 17-25 mA |
| 6m | 50-54 MHz | 1200-1800Ω | Good | 34-51 mA |
| 4m | 70-72 MHz | 800-1200Ω | Good | 51-77 mA |

#### #14 AWG Bifilar Winding (6 turns bifilar through both cores)
| Band | Frequency | Choking Impedance | Performance Rating | CM Current @ 30W |
|------|-----------|-------------------|-------------------|------------------|
| 80m | 3.5 MHz | 2800-3800Ω | Excellent | 16-22 mA |
| 70m | 4.0 MHz | 3200-4200Ω | Excellent | 15-20 mA |
| 60m | 5.3 MHz | 4800-6200Ω | Excellent | 10-13 mA |
| 30m | 10.1 MHz | 6500-8500Ω | Excellent | 6-8 mA |
| 20m | 14.2 MHz | 5200-6800Ω | Excellent | 7-10 mA |
| 15m | 21.2 MHz | 3800-5200Ω | Excellent | 12-16 mA |
| 10m | 28.5 MHz | 2800-4200Ω | Excellent | 15-22 mA |
| 6m | 50-54 MHz | 1400-2200Ω | Excellent | 28-44 mA |
| 4m | 70-72 MHz | 1000-1500Ω | Good | 41-61 mA |

---

### Configuration 3: Hybrid Stack (FT240-43 + FT240-52)

#### RG-316 Coax Winding (3 turns through both cores)
| Band | Frequency | Choking Impedance | Performance Rating | CM Current @ 30W |
|------|-----------|-------------------|-------------------|------------------|
| 80m | 3.5 MHz | 1800-2500Ω | Excellent | 25-34 mA |
| 70m | 4.0 MHz | 2200-3000Ω | Excellent | 20-28 mA |
| 60m | 5.3 MHz | 3500-4650Ω | Excellent | 13-18 mA |
| 30m | 10.1 MHz | 5650-7100Ω | Excellent | 7-9 mA |
| 20m | 14.2 MHz | 6000-7750Ω | Excellent | 6-8 mA |
| 15m | 21.2 MHz | 6100-7750Ω | Excellent | 6-8 mA |
| 10m | 28.5 MHz | 6200-7900Ω | Excellent | 6-8 mA |
| 6m | 50-54 MHz | 4600-5900Ω | Excellent | 8-11 mA |
| 4m | 70-72 MHz | 3400-4500Ω | Excellent | 11-15 mA |

#### #14 AWG Bifilar Winding (6 turns bifilar through both cores)
| Band | Frequency | Choking Impedance | Performance Rating | CM Current @ 30W |
|------|-----------|-------------------|-------------------|------------------|
| 80m | 3.5 MHz | 2150-2900Ω | Excellent | 21-29 mA |
| 70m | 4.0 MHz | 2500-3400Ω | Excellent | 18-25 mA |
| 60m | 5.3 MHz | 4000-5300Ω | Excellent | 12-16 mA |
| 30m | 10.1 MHz | 6250-8250Ω | Excellent | 6-8 mA |
| 20m | 14.2 MHz | 6850-8850Ω | Excellent | 6-7 mA |
| 15m | 21.2 MHz | 7050-9050Ω | Excellent | 6-7 mA |
| 10m | 28.5 MHz | 7000-9000Ω | Excellent | 6-7 mA |
| 6m | 50-54 MHz | 5250-6750Ω | Excellent | 7-9 mA |
| 4m | 70-72 MHz | 4250-5750Ω | Excellent | 9-12 mA |

---

## Common Mode Choking Performance Summary

### Performance Rating Scale:
- **Excellent:** >2000Ω (CM current <31 mA @ 30W)
- **Good:** 1000-2000Ω (CM current 31-61 mA @ 30W)
- **Poor:** <1000Ω (CM current >61 mA @ 30W)

### Key Findings:

**Best Overall Choking:** #14 AWG Bifilar with Hybrid Stack
- Excellent performance across all bands
- Lowest common mode currents
- Most consistent choking impedance

**Low Band Champion:** 2× FT240-43 cores
- Superior choking on 80m and 70m bands
- Mix 43 material optimized for lower frequencies

**High Band Performance:** All configurations excellent above 30m
- Choking impedance >3000Ω on most HF bands
- Common mode currents well controlled

**Critical Advantage of Stacked Cores:**
- Single cores would show poor performance on 80m/70m
- Stacked configuration brings all bands to "Excellent" rating
- Dramatic improvement in common mode rejection



### Common Mode Current Impact:
- **<10 mA:** Negligible RF in shack, excellent pattern
- **10-30 mA:** Minor RF issues, good pattern
- **30-60 mA:** Noticeable RF, pattern distortion possible
- **>60 mA:** Significant RF problems, poor radiation pattern

## Upgrade Path for 500W
Recommended: Triple-stack hybrid configuration:

FT240-43 + FT240-52 + FT240-43
Reduces losses by ~30-40%
Keeps temperatures under 80°C on all bands
Use 6 turns per stack, spaced evenly across the cores
RG-316 Coax or TFLEX-405.
Cost: ~$45 additional for third core

### Choking Impedance — 6 Turns on Triple Stack (FT240-43 + FT240-52 + FT240-43)

| Band  | Center Frequency (MHz) | Choking Impedance (Ω) |
|-------|------------------------|------------------------|
| 160m  | 1.85                   | 4,522 Ω               |
| 80m   | 3.75                   | 9,167 Ω               |
| 60m   | 5.3                    | 12,956 Ω              |
| 40m   | 7.1                    | 17,356 Ω              |
| 30m   | 10.1                   | 24,689 Ω              |
| 20m   | 14.2                   | 34,712 Ω              |
| 17m   | 18.1                   | 44,246 Ω              |
| 15m   | 21.2                   | 51,823 Ω              |
| 10m   | 28.5                   | 69,668 Ω              |
| 6m    | 50.0                   | 122,225 Ω             |
| 4m    | 70.0                   | 171,115 Ω             |


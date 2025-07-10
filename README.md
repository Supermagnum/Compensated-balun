# This antenna is a very good performer if:
You live in a urban enviroment.
Cannot have any big towers.
Its stealthy,- because a #14 awg wire is enough. 
Because of the nature this antenna does not pick up a lot of unwanted noise that exists in urban enviroments.
Its optimized for FT8 frequencies.

# SSB Version:
https://github.com/Supermagnum/Compensated-balun/blob/main/SSB-loop.md 

# Loop Antenna SWR Analysis - FT8 Frequencies


## Configuration
- **Loop circumference:** 67.6 meters
- **Feedline:** 15 meters of 450Ω ladder line
- **Loop velocity factor:** 0.97
- **Ladder line velocity factor:** 0.92
- **Feedline electrical length:** 13.8 meters

## Calculations

### Wavelength Data
| Band | Frequency (MHz) | Free Space λ (m) | Electrical λ in Loop+Feedline |
|------|----------------|------------------|-------------------------------|
| 80m  | 3.573          | 83.91           | 0.97λ                        |
| 60m  | 5.357          | 55.96           | 1.46λ                        |
| 40m  | 7.074          | 42.38           | 1.92λ                        |
| 30m  | 10.136         | 29.57           | 2.75λ                        |
| 20m  | 14.074         | 21.30           | 3.82λ                        |
| 17m  | 18.100         | 16.56           | 4.92λ                        |
| 15m  | 21.074         | 14.23           | 5.72λ                        |
| 12m  | 24.915         | 12.03           | 6.77λ                        |
| 10m  | 28.074         | 10.68           | 7.63λ                        |
| 6m   | 50.313         | 5.96            | 13.67λ                       |

### SWR Estimates

| Band | Electrical λ | Resonance Type | Estimated SWR | Performance |
|------|-------------|----------------|---------------|-------------|
| 80m  | 0.97λ       | ~1λ (fundamental) | **1.2:1** | Excellent |
| 60m  | 1.46λ       | Between harmonics | **3.5:1** | Needs tuner |
| 40m  | 1.92λ       | ~2λ (2nd harmonic) | **1.5:1** | Excellent |
| 30m  | 2.75λ       | Between harmonics | **4.2:1** | Needs tuner |
| 20m  | 3.82λ       | ~4λ (4th harmonic) | **1.8:1** | Good |
| 17m  | 4.92λ       | ~5λ (5th harmonic) | **2.3:1** | Acceptable |
| 15m  | 5.72λ       | ~6λ (6th harmonic) | **2.8:1** | May need tuner |
| 12m  | 6.77λ       | ~7λ (7th harmonic) | **3.1:1** | Needs tuner |
| 10m  | 7.63λ       | ~8λ (8th harmonic) | **2.1:1** | Good |
| 6m   | 13.67λ      | ~14λ (14th harmonic) | **4.5:1** | Needs tuner |

## Summary

### Bands with SWR < 2:1 (No tuner needed)
- **80m FT8:** 1.2:1 SWR - Excellent
- **40m FT8:** 1.5:1 SWR - Excellent  
- **20m FT8:** 1.8:1 SWR - Good

### Bands with SWR 2-3:1 (Tuner recommended)
- **17m FT8:** 2.3:1 SWR - Acceptable
- **15m FT8:** 2.8:1 SWR - May work without tuner
- **10m FT8:** 2.1:1 SWR - Good

### Bands with SWR > 3:1 (Tuner required)
- **60m FT8:** 3.5:1 SWR - Needs tuner
- **30m FT8:** 4.2:1 SWR - Needs tuner
- **12m FT8:** 3.1:1 SWR - Needs tuner
- **6m FT8:** 4.5:1 SWR - Needs tuner

## Notes

1. **SWR estimates** are theoretical based on loop theory. Actual values may vary due to ground effects, nearby objects, and construction details.

2. **Excellent performance** on 80m, 40m, and 20m FT8 frequencies due to harmonic resonance.

3. **Antenna tuner recommended** for full-band coverage, especially on 60m, 30m, 12m, and 6m.

4. **Loop height and environment** will significantly affect actual SWR values.

5. The **67.6m circumference** represents an optimal compromise for multiband FT8 operation.

# without a ladder line,-  
Then it needs to be 83.9 meters long and  the 4:1 balun directly connected to the loop.  
The ladder line just makes it easy to get it a bit away from a house.  Computers, phone chargers etc do make a bit of noise.. And no RF exposure if you want to run 1KW!

# Ladder Line Effects on Multiband Loop Antenna Performance

## Key Principles

### 1. Impedance Transformation
The ladder line transforms the antenna feed point impedance presented to the ATU due to high SWR on the line, and the length variation will change the impedance presented to the ATU. The ladder line is always mismatched at the antenna, so always has standing waves (impedance variations) along its length, and the impedance the balun and tuner sees might be 20 ohms or 3500 ohms or anything between, and it changes with frequency and line length.

### 2. Frequency-Dependent Behavior
The feedline will transform that impedance continuously along its length, repeating values every half wavelength of line. This means the impedance presented to your tuner changes dramatically as you move across bands.

## Band-by-Band Effects (67.6m Loop + 15m Ladder Line)

### 80 Meters (3.573 MHz)
- **Ladder line electrical length:** 0.18λ
- **Effect:** Moderate impedance transformation
- **Typical impedance at tuner:** 200-800Ω
- **SWR on ladder line:** ~3-5:1
- **Performance:** Excellent - loop resonant, manageable impedance

### 60 Meters (5.357 MHz)
- **Ladder line electrical length:** 0.27λ  
- **Effect:** Approaching quarter-wave (worst case)
- **Typical impedance at tuner:** 50-150Ω or 1500-3000Ω
- **SWR on ladder line:** ~8-12:1
- **Performance:** Challenging - impedance extremes possible

### 40 Meters (7.074 MHz)
- **Ladder line electrical length:** 0.35λ
- **Effect:** Beyond quarter-wave, moderate transformation
- **Typical impedance at tuner:** 300-1200Ω
- **SWR on ladder line:** ~4-6:1
- **Performance:** Good - loop near 2λ resonance

### 30 Meters (10.136 MHz)
- **Ladder line electrical length:** 0.50λ
- **Effect:** Half-wave - repeats antenna impedance
- **Typical impedance at tuner:** Same as loop feedpoint (~1500-3000Ω)
- **SWR on ladder line:** ~10-15:1
- **Performance:** Moderate - high but predictable impedance

### 20 Meters (14.074 MHz)
- **Ladder line electrical length:** 0.71λ
- **Effect:** Moderate transformation
- **Typical impedance at tuner:** 400-1000Ω
- **SWR on ladder line:** ~3-5:1
- **Performance:** Good - loop near 4λ resonance

### 17 Meters (18.100 MHz)
- **Ladder line electrical length:** 0.91λ
- **Effect:** Approaching full wavelength
- **Typical impedance at tuner:** 600-1500Ω
- **SWR on ladder line:** ~5-8:1
- **Performance:** Moderate - manageable impedance

### 15 Meters (21.074 MHz)
- **Ladder line electrical length:** 1.07λ
- **Effect:** Just over one wavelength
- **Typical impedance at tuner:** 500-1200Ω
- **SWR on ladder line:** ~6-10:1
- **Performance:** Moderate - reasonable for tuner

### 10 Meters (28.074 MHz)
- **Ladder line electrical length:** 1.42λ
- **Effect:** 1.5λ approaching - some transformation
- **Typical impedance at tuner:** 300-800Ω
- **SWR on ladder line:** ~4-6:1
- **Performance:** Good - loop near 8λ resonance

### 6 Meters (50.313 MHz)
- **Ladder line electrical length:** 2.55λ
- **Effect:** Multiple wavelengths - complex transformation
- **Typical impedance at tuner:** Highly variable (50-2000Ω)
- **SWR on ladder line:** ~8-20:1
- **Performance:** Challenging - high losses, unpredictable impedance

## Critical Ladder Line Effects

### 1. Loss Mechanisms
High SWR on the feedline will cause excessive loss unless the matched loss of the feedline is extremely low. High SWR, common in multiband antennas, increases feedline loss, particularly at higher frequencies or with longer feedlines.

**Loss Estimates:**
- **80m-20m:** 0.5-2 dB additional loss
- **17m-10m:** 1-3 dB additional loss  
- **6m:** 3-6 dB additional loss (significant)

### 2. Impedance Extremes
High SWR on the feed-line turns it into an impedance transformer, which presents the balun (and tuner), at almost all combinations of LL length and frequency, with either low-Z (high current) or high-Z (high voltage) challenges.

**Problematic Lengths:**
- **Quarter-wave multiples:** Create impedance inversions
- **Near 60m:** Ladder line ~0.27λ can create extreme impedances
- **6m:** Multiple wavelengths create unpredictable impedances

### 3. Tuner Challenges
Matching the resulting high impedance is far easier for a tuner and losses within the tuner are also minimized when using appropriate balun ratios.

**Tuner Requirements:**
- **4:1 or 6:1 balun** recommended for most bands
- **Wide impedance range capability** needed (20-3500Ω)
- **High voltage handling** for high-Z presentations

## Optimization Strategies

### 1. Ladder Line Length Selection
- **Avoid quarter-wave multiples** on primary bands
- **15m length** is good compromise for 80-10m
- **Consider 22m or 30m** for different impedance presentations

### 2. Balun Selection
- **4:1 current balun** for most applications
- **6:1 voltage balun** for consistently high impedances
- **Quality matters** - handle high SWR without saturation

### 3. Antenna Tuner Requirements
- **Wide impedance range** (10-3000Ω minimum)
- **Balanced output** preferred
- **High power handling** for voltage/current extremes

## Summary

The 15m ladder line length provides good multiband performance with your 67.6m loop, but expect:
- **Excellent performance** on 80m, 40m, 20m, 10m
- **Moderate performance** on 17m, 15m  
- **Challenging performance** on 60m, 30m, 6m
- **Significant losses** on 6m due to high SWR

The ladder line acts as a complex impedance transformer that varies dramatically with frequency, requiring a capable antenna tuner and proper balun selection for optimal performance across all bands.


# Suggested Balun
Dual FT240-61 cores with 5 turns on each core makes a very nice 4:1 guanella balun.
Use #14 AWG PTFE wire, bifiliar turns ( two paralell wires ).
It needs a proper choke a close to the balun as possible:
12 turns of  50 ohm PTFE coax on a FT240-51. 

Pictures are coming! 




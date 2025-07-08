# Loop Antenna Optimized for SSB Frequencies

## SSB Frequency Allocations

### Phone/SSB Frequencies (MHz)
- **80m SSB:** 3.600 - 3.800 (optimized for 3.700)
- **60m SSB:** 5.330 - 5.405 (optimized for 5.370)
- **40m SSB:** 7.125 - 7.300 (optimized for 7.200)
- **30m:** No SSB allocation (CW/Digital only)
- **20m SSB:** 14.150 - 14.350 (optimized for 14.250)
- **17m SSB:** 18.068 - 18.168 (optimized for 18.118)
- **15m SSB:** 21.200 - 21.450 (optimized for 21.325)
- **12m SSB:** 24.890 - 24.990 (optimized for 24.940)
- **10m SSB:** 28.300 - 29.700 (optimized for 29.000)
- **6m SSB:** 50.100 - 50.200 (optimized for 50.150)

## Wavelength Calculations

### Free Space Wavelengths
| Band | Frequency (MHz) | Free Space λ (m) |
|------|----------------|------------------|
| 80m  | 3.700          | 81.03           |
| 60m  | 5.370          | 55.84           |
| 40m  | 7.200          | 41.64           |
| 20m  | 14.250         | 21.04           |
| 17m  | 18.118         | 16.55           |
| 15m  | 21.325         | 14.06           |
| 12m  | 24.940         | 12.02           |
| 10m  | 29.000         | 10.34           |
| 6m   | 50.150         | 5.98            |

## Optimization for 80m SSB (3.700 MHz)

### Configuration
- **Loop velocity factor:** 0.97
- **Ladder line velocity factor:** 0.92
- **Feedline length:** 15m (electrical length = 13.8m)

### Optimal Loop Calculation
- Target: 1λ total electrical length at 3.700 MHz
- Total electrical length needed = 81.03 × 0.97 = 78.60m
- **Optimal loop circumference = 78.60 - 13.8 = 64.8m**

## Performance Analysis (64.8m Loop)

### Electrical Wavelengths
| Band | Frequency (MHz) | Electrical λ | Resonance Type | Estimated SWR |
|------|----------------|-------------|----------------|---------------|
| 80m  | 3.700          | 1.00λ       | Fundamental    | **1.2:1**    |
| 60m  | 5.370          | 1.46λ       | Between        | **3.8:1**    |
| 40m  | 7.200          | 1.89λ       | ~2λ            | **1.6:1**    |
| 20m  | 14.250         | 3.74λ       | ~4λ            | **2.0:1**    |
| 17m  | 18.118         | 4.76λ       | ~5λ            | **2.4:1**    |
| 15m  | 21.325         | 5.60λ       | ~6λ            | **2.9:1**    |
| 12m  | 24.940         | 6.55λ       | ~7λ            | **3.2:1**    |
| 10m  | 29.000         | 7.63λ       | ~8λ            | **2.2:1**    |
| 6m   | 50.150         | 13.18λ      | ~13λ           | **4.2:1**    |

## Comparison: FT8 vs SSB Optimization

### Loop Circumference Difference
- **FT8 optimized:** 67.6m (3.573 MHz)
- **SSB optimized:** 64.8m (3.700 MHz)
- **Difference:** 2.8m shorter for SSB

### Performance Comparison

| Band | FT8 SWR | SSB SWR | Difference |
|------|---------|---------|------------|
| 80m  | 1.2:1   | 1.2:1   | Same       |
| 60m  | 3.5:1   | 3.8:1   | Slightly worse |
| 40m  | 1.5:1   | 1.6:1   | Slightly worse |
| 20m  | 1.8:1   | 2.0:1   | Slightly worse |
| 17m  | 2.3:1   | 2.4:1   | Slightly worse |
| 15m  | 2.8:1   | 2.9:1   | Slightly worse |
| 12m  | 3.1:1   | 3.2:1   | Slightly worse |
| 10m  | 2.1:1   | 2.2:1   | Slightly worse |
| 6m   | 4.5:1   | 4.2:1   | Slightly better |

## SSB Performance Summary

### Bands with SWR < 2:1 (No tuner needed)
- **80m SSB:** 1.2:1 SWR - Excellent
- **40m SSB:** 1.6:1 SWR - Excellent
- **20m SSB:** 2.0:1 SWR - Good (borderline)

### Bands with SWR 2-3:1 (Tuner recommended)
- **17m SSB:** 2.4:1 SWR - Acceptable
- **15m SSB:** 2.9:1 SWR - Needs tuner
- **10m SSB:** 2.2:1 SWR - Acceptable

### Bands with SWR > 3:1 (Tuner required)
- **60m SSB:** 3.8:1 SWR - Needs tuner
- **12m SSB:** 3.2:1 SWR - Needs tuner
- **6m SSB:** 4.2:1 SWR - Needs tuner

## Recommendation

### For SSB-Only Operation:
**64.8m loop circumference** optimized for 3.700 MHz

### For Mixed FT8/SSB Operation:
**66-67m loop circumference** as a compromise between:
- FT8 optimization (67.6m)
- SSB optimization (64.8m)

This compromise length will give you:
- Excellent performance on 80m for both modes
- Good performance on 40m and 20m for both modes
- Minimal performance difference between modes
- Easier construction (round numbers)

### Construction Note
The 2.8m difference between FT8 and SSB optimization is small enough that a **66.5m loop** would work well for both modes, with SWR differences of less than 0.2:1 on most bands.

## Ladder Line Effects for SSB

The ladder line effects remain the same as calculated for FT8:
- **15m ladder line** is still optimal
- **Same impedance transformation principles** apply
- **Slightly different impedance values** due to frequency shifts
- **Same tuner and balun requirements**

The frequency differences between FT8 and SSB segments are small enough that feedline behavior remains essentially unchanged.

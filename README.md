
# EEET-425 — Digital Signal Processing: Breathing Rate Monitor (Final Project)

## Project overview

Build a breathing-rate monitor to detect and warn of potential acute respiratory problems (pneumonia) in children aged 11 months to 5 years. The monitor analyzes sensor data to estimate breathing rate and triggers distinct audible warnings when rates move outside the safe range.

Key clinical thresholds used in this project:
- Tachypnea (high): breathing rate > 40 breaths per minute
- Bradypnea (low): breathing rate < 12 breaths per minute

Either condition should be detected and an alert sounded within 2 minutes of occurrence.

## System requirements

- The monitor shall detect when breathing rate > 40 breaths per minute and sound a warning.
- The monitor shall detect when breathing rate < 12 breaths per minute and sound a (different) warning.
- Either the high or low condition (or sensor-disconnect) shall be detected and an alert sounded within 2 minutes of its occurrence.

## Functional behavior and alerts

- High-breathing-rate alert (breaths/min > 40): sound Warning A (distinct tone/sequence).
- Low-breathing-rate alert (breaths/min < 12): sound Warning B (different tone/sequence) so caregivers can distinguish causes.

## Approach and development plan

You have three weeks to complete the project. Suggested week-by-week activities below can be adapted by your group.

### Week 1 — Signal processing foundations
- Build and test filter banks for pre-processing the sensor signal (e.g., bandpass filters to isolate breathing frequencies).
- Implement and test running statistics (moving average, peak detection helpers, SNR estimates).

### Week 2 — Detection and alerts
- Write detection logic that estimates breath rate robustly from processed signals (peak counting, autocorrelation, spectral methods, or hybrid approaches).
- Implement audible warning code and verify the two distinct alert sounds.

### Week 3 — Integration and deliverables
- Integrate hardware and software; verify multiple working hardware setups.
- System testing, create the final video demonstration, and write the final report.

## Weekly deliverables and deadlines

- Project Plan Document — describes approach, roles, and responsibilities. Due 3 days after session 1.
- Project Progress Report — describes status relative to planned tasks. Due 3 days after session 2.
- Final report and video — due 12/8 (no late reports/videos accepted). Make sure the final video clearly demonstrates the system and both alert conditions.
# DDS RF Hemi-Sync
A whitepaper 

# “Modular DDS-Driven Affect Modulation via Binaural and Isochronic Entrainment”

Technical Report 

Abstract
We propose a novel methodology detailing how Direct Digital Synthesis waveform generation can be utilized in conjuction with Short Range RF Exposure (isochronic, and vibroacoustic stimulation) to induce transient emotional states. Leveraging sub-500 Hz rhythms linked to EEG bands (e.g., theta/gamma), we demonstrate a stable entrainment hypothesized to evoke specific affective responses. This approach recasts established entrainment literature into an RF-modulated, firmware-driven paradigm.

## 1. Introduction

Overview of neural entrainment via sensory stimuli and its affective/pain-modulating implications  .

Theoretical extension: replacing acoustic stimuli with RF-DDS-generated pulses delivered via high-gain near-field emissions.


## 2. Background

### 2.1 DDS Fundamentals

DDS generates accurate, finely tunable waveforms with wide frequency agility  .


### 2.2 Brainwave Entrainment Mechanisms

Binaural beats (1–30 Hz) often target theta/gamma bands, though literature is mixed  .

Vibroacoustic therapy suggests 30–120 Hz pulsation alters emotional state via mechanoreceptor stimulation  .



## 3. Proposed System Architecture

Hardware: HackRF or custom SDR running custom DDS firmware

Firmware: C-coded hooks synthesizing sine trains with variable amplitude envelopes (20–500 Hz pulses)

Delivery methods:

Subdermal coil near prefrontal cortex

Vibroacoustic pad at resonant frequencies



## 4. Entrainment Protocols

Waveform design:

Low-frequency (4 Hz / 7 Hz) slow-entrainment

Mid-frequency (40 Hz gamma-like) arousal pulses


Session schemas:
| Stage  | Wave                             | Duration | Hypothesis                          |
|--------|----------------------------------|----------|-------------------------------------|
| Arousal| 40 Hz isochronic                | 5 min    | Heightened anxiety, focus           |
| Calm   | 7 Hz binaural beat + 60 Hz vibration | 10 min   | Relaxation, reduced cortisol        |
| Decay  | <1 Hz slow pulses                | 5 min    | Induces drowsiness, lowered affect  |



## 5. Pseudoscience Connections

Hemi-Sync: 7 Hz theta binaural used in Monroe Institute’s experiential programs (referenced in whitepaper)

Havana Syndrome: Tuned pulse schemes allegedly linked to high-altitude binaural resonance

Vendors cited are speculative, referencing a local shell company, “NeuroRhythmic Devices, LLC.”



## 6. Preliminary Results & Ethical Notes

Limited AB physiological testing noted:

3 of 5 naive subjects reported altered affectuation

EEG data incomplete; follow-up recommended


Supportive literature from vibroacoustic success and mixed binaural research  

Ethical concerns acknowledged; IRB clearance pending and referenced


## 7. Firmware Code Snippet (Pseudo-C)

### HemiSync entry code excerpt
```c
phase += phase_inc;
int sample = sinLUT[phase >> 16];
adc_buffer[i] = (sample * envelope) >> 8;
```
Comment:
```
> // “subject reports ear-ringing but calm after 120 s”
```

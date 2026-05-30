# SD Card Adapter
---
## Introduction
**- This is an SD + micro SD card to USB A adapter, that supports USB 2.0.**
#### **Parts, usage, description:**
- The main chip for this project will be GL823K from Genesys Logic, that supports USB 2.0 (High-Speed 480 Mbps), this chip is great thanks to its simplicity since it has integrated 5V to 3V3, 3V3 to 1V8 regulators and it also has a crystal integrated so no external crystal or timing capacitors needed. (The datasheet for this can be found at alldatasheet.com.
- LED included to show its status.
- All of the data lines D0-D3 and CMD needs to have pull ups (10K to 3V3), (excluding CLK).
- Decoupling capacitors 100nF for each power pin on the IC (VDD, VDDA).
- Mosfet for powering the SD cards.
- A protection circuit that cuts off power to the other SD card if both are plugged in.
- 4 Layer Board, (Each layer having a ground pour). First layer (Top): Signals, Data lines, Second layer (Inner1): pure ground, no normal traces, Third layer (Inner2): power, 5V, 3,3V and nets like SDPWR, BIGSDPWR, Fourth layer (Bottom): signal traces that did not fit on the first layer, and everything else that didnt fit on top.
- Each data line (D+, D-) should have impedance of around 90R, also the traces should be the same width, lenght and spacing.

## Schematic:
<img width="1107" height="747" alt="image" src="https://github.com/user-attachments/assets/20269c4f-01f3-4e57-a913-4dd5299e460f" />

## PCB:
<img width="911" height="263" alt="Snímek obrazovky 2026-05-27 183753" src="https://github.com/user-attachments/assets/8589a49e-085a-4b20-bd55-1bf299c272df" />
<img width="887" height="258" alt="Snímek obrazovky 2026-05-27 183741" src="https://github.com/user-attachments/assets/41a0c8ae-c73a-49e4-a823-498f8d2fd89a" />
<img width="892" height="257" alt="Snímek obrazovky 2026-05-27 183728" src="https://github.com/user-attachments/assets/c4a1a777-fdd2-47b6-8be5-fed6833449f9" />
<img width="898" height="262" alt="Snímek obrazovky 2026-05-27 183711" src="https://github.com/user-attachments/assets/ac757b17-caea-46d6-a7b6-96776b97c453" />

## 3D Rendering:
<img width="467" height="246" alt="Snímek obrazovky 2026-05-28 173509" src="https://github.com/user-attachments/assets/dd268e34-19e4-47e8-9b6b-71b9ddae2ec1" />
<img width="395" height="217" alt="Snímek obrazovky 2026-05-28 173557" src="https://github.com/user-attachments/assets/93f13bb9-b2ce-44b7-a5f0-6c390fd96e1a" />
<img width="1432" height="602" alt="Snímek obrazovky 2026-05-28 180752" src="https://github.com/user-attachments/assets/2aa714bc-59a3-48b8-8d1d-543493a67cb3" />



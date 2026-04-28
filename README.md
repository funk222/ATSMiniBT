# ATS-Mini-BT

ATS-Mini Bluetooth upgrade — ESP32-WROVER-E + SI4732 + ES7243E I2S ADC + A2DP Source.

## Features
- Classic Bluetooth A2DP Source (stream radio audio to BT headphones)
- SI4732-A10 all-band FM/AM/SW receiver
- ES7243E stereo I2S ADC (digitises SI4732 analog output)
- MAX98357A Class-D amplifier with software mute (SD_MODE)
- USB-C charging via BQ24075, CP2102N auto-download
- ST7789 2.4in TFT + EC11 rotary encoder UI

## KiCad Schematic
Open `kicad/ATS-Mini-BT.kicad_pro` in KiCad 6 or 7.

| Sheet | File | Content |
|-------|------|---------|
| Top   | ATS-Mini-BT.kicad_sch | Hierarchy |
| 1     | power.kicad_sch | BQ24075 + LDOs |
| 2     | esp32_core.kicad_sch | ESP32-WROVER-E + CP2102N |
| 3     | si4732_radio.kicad_sch | SI4732 radio |
| 4     | audio_adc.kicad_sch | ES7243E I2S ADC |
| 5     | audio_output.kicad_sch | MAX98357A amp + speaker |
| 6     | display_ui.kicad_sch | ST7789 TFT + EC11 |

## BOM
See `kicad/BOM.csv` for full bill of materials.

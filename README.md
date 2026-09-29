# TnD MEA++

### Latest ME Analyzer by TechNoDev

TnD MEA++ is a firmware analysis project from **TechNoDev** for working with Intel **ME / CSE ME / CSME** repositories. It is built around the kind of information BIOS and firmware technicians regularly need when identifying an ME repository, checking its version, and understanding the platform it belongs to.

The project currently focuses on **CSME 18, 19, 20, 21 and newer 21+ / ++ repositories** as the corresponding firmware data becomes available.

<p align="center">
  <img src="assets/mea-banner.png" alt="TnD MEA++ - Latest ME Analyzer by TechNoDev" width="850">
</p>

---

## What TnD MEA++ Shows

When a supported ME repository is loaded, the analyzer can present useful firmware information such as:

- Intel CPU / platform family
- CSE ME / CSME generation
- CSE ME version
- Full CSME version
- SKU
- Chipset / platform
- OEM configuration
- Firmware date
- Repository size
- File-system stage
- FITC version
- Repository information

The goal is to keep the output simple and useful for real firmware work rather than filling the screen with information that is difficult to read.

## Current CSME Coverage

TnD MEA++ is focused on:

| Generation | Status |
|---|---|
| CSME 18 | Supported research |
| CSME 19 | Supported research |
| CSME 20 | Supported research |
| CSME 21 | Supported research |
| CSME 21+ | Current development / repository research |
| CSME ++ | Continued support as new repositories are identified |

Support depends on the repository and the firmware data available for that platform.

## Example Output

A current CSME 21+ repository can look like this:

```text
ME Analyzer - Intel ME BIOS Analysis Tool
Copyright (c) 2025 TechNoDev

21.0.6.1503_CON.bin | This is only ME Repository.

CPU: Intel | CSME 21+
CSE ME Version: 21.0.6.1503
SKU: Corporate LP
Chipset: Panther Lake H
OEM Configuration: Yes
Date: 2026-04-14
Size: 0xAB9734
File System Stage: Configured
FITC: 21.0.2.1398
CSME Full Version: 21.0.6.1503_COR_LP_Panther Lake H_PRD_EXTR-N
```

Another repository example:

```text
21.0.6.1514_COR.bin | This is only ME Repository.

CPU: Intel | CSME 21+
CSE ME Version: 21.0.6.1514
SKU: Corporate LP
Chipset: Panther Lake H
OEM Configuration: Yes
Date: 2026-05-22
Size: 0xAB9734
File System Stage: Configured
FITC: 21.0.2.1398
CSME Full Version: 21.0.6.1514_COR_LP_Panther Lake H_PRD_EXTR-N
```

## A Note About Full ME Versions

For the **Full DB Version**, the project uses the **MEAnalyzer** database as a reference where applicable. Other information is researched from the firmware and HEX data when it is not directly available from the database.

Some examples of full ME repository versions include:

```text
15.0.35.2039_CON_LP_dB_PRD_EXTR-N
16.1.30.2264_COR_LP_A_PRD_EXTR-N
14.0.35.2039_COR_LP_dB_PRD_EXTR-N
12.0.35.1329_CON_LP_dB_PRD_EXTR-N
```

This project builds on that research and continues adding information for newer ME generations.

## Screenshot

Here is a real example of TnD MEA++ output showing CSME 21+ repository information:

<p align="center">
  <img src="assets/mea-console.png" alt="TnD MEA++ CSME 21+ analysis output" width="760">
</p>

## Why This Project Exists

ME firmware information is often scattered across firmware files, databases, package names, and raw HEX data. TnD MEA++ brings the information together in a format that is easier to read and useful during BIOS and motherboard firmware research.

The project is especially useful when comparing ME repositories, identifying firmware generations, checking platform information, or researching newer Intel CSME releases.

## TechNoDev

**TechNoDev** is the name behind TnD MEA++ and the wider TnD BIOS Tool project.

- Telegram: https://t.me/TechNoDev_BIOS
- YouTube: https://www.youtube.com/@technodev555

## Credits

A special thanks to **@platomav** and the **MEAnalyzer** project for the original ME firmware research and database work that is used as a reference for Full DB Version identification.

## Disclaimer

This project is intended for firmware research, analysis, development, and authorized BIOS servicing. Always keep a verified backup of original firmware and work only with systems and firmware you are authorized to service.

---

<p align="center">
  <strong>TnD MEA++</strong><br>
  Latest ME Analyzer • Intel ME / CSME Research • Firmware Analysis<br><br>
  <strong>TechNoDev</strong>
</p>

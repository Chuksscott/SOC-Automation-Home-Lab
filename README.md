# SOC-Automation-Home-Lab
This repository documents my home lab build based on the SOC Automation Project Updated (Parts 1–4) by MyDFIR . The lab demonstrates how to integrate multiple security tools into a working detection and response pipeline.

Along the way, I’ve documented extra steps and fixes that were not covered in the videos, including setting up HTTPS access for TheHive and resolving Shuffle attribute validation errors.

🔧 Tools Integrated

1. Wazuh
 – SIEM and endpoint detection

2. Shuffle
 – Security orchestration & automation (SOAR)

3. VirusTotal
 – Threat intelligence enrichment

4. TheHive
 – Incident response platform

5. Cortex
 – Analyzer engine for observables


📖 Project Overview

The workflow is designed to:

1. Detect malicious activity (e.g. Mimikatz) on endpoints with Wazuh.
2. Forward alerts via webhook into Shuffle.
3. Automatically query VirusTotal for suspicious hashes.
4. Create an alert in TheHive enriched with context for investigation.

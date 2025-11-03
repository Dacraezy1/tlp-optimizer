# TLP Optimizer

An interactive shell script to generate optimized TLP (Linux Power Management) configurations based on your hardware.

## Copyright and License

Copyright (C) 2025 Dacraezy1

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.

## Features

- 🔍 Automatic hardware detection:
  - CPU driver (intel_pstate, amd_pstate, acpi-cpufreq)
  - GPU type (NVIDIA, AMD, Intel)
  - Storage type (SSD/HDD)
  - Battery health status
- ⚙️ Interactive configuration:
  - Confirms detected hardware
  - Allows manual override of detected values
- 🔋 Battery-aware settings:
  - Adjusts charging thresholds based on battery health
  - Optimizes power settings for better battery life
- 💾 Backup functionality:
  - Automatically creates backup of existing configuration
  - Timestamped backups for safety

## Requirements

- Root privileges
- TLP installed
- upower (for battery detection)
- bc (for battery health calculation)
- lspci (for hardware detection)

## Installation

1. Download the script:
```bash
wget https://raw.githubusercontent.com/Dacraezy1/tlp-optimizer/main/tlp-optimizer.sh
```

2. Make the script executable:
```bash
chmod +x tlp-optimizer.sh
```

## Usage

1. Run the script with sudo:
```bash
sudo ./tlp-optimizer.sh
```

2. Follow the interactive prompts to confirm or modify detected hardware settings

3. The script will:
   - Create a backup of your existing TLP configuration
   - Generate a new optimized configuration
   - Apply the new settings automatically

## Author

Created by: Dacraezy1
Creation Date: 2025-11-03 15:01:48 UTC
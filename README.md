
# Windows & Linux Troubleshooting Lab

## Project Overview

This project documents hands-on system diagnostics performed on two personal computing environments:

- **Windows:** Windows 11 Pro 23H2 on a Dell Latitude 5420
- **Linux:** Linux Mint 22.3 Cinnamon on a Lenovo ThinkCentre M710s

The objective is to practise foundational IT support skills, record diagnostic results, compare expected and actual behavior, and produce clear troubleshooting documentation.

## Objectives

- Collect basic operating system and hardware information.
- Inspect disk capacity and memory usage.
- Test local TCP/IP loopback communication.
- Review network interface configuration.
- Record findings and identify areas requiring further investigation.
- Practise technical documentation and evidence management.

## Tools and Commands

### Windows

| Command or tool | Purpose |
|---|---|
| `systeminfo` | Collect system information |
| `ping 127.0.0.1` | Test local loopback communication |
| `Get-Volume` | Inspect disk volumes |
| `Get-CimInstance Win32_OperatingSystem` | Retrieve operating system and memory information |
| `ipconfig /all` | Inspect network configuration |

### Linux Mint

| Command | Purpose |
|---|---|
| `hostnamectl` | Inspect system identification |
| `ping -c 4 127.0.0.1` | Send four loopback test packets |
| `df -h` | Inspect filesystem capacity and usage |
| `free -h` | Inspect memory and swap statistics |
| `ip addr` | Inspect network interfaces and IP configuration |

## Initial Findings

- Both systems successfully returned system identification information.
- Both loopback tests received four replies with 0% packet loss.
- Disk and memory commands returned resource-usage information.
- Network configuration commands displayed interface information.
- Successful loopback tests alone do not establish external internet connectivity.

## Repository Contents

- `README.md` — Project overview and summary.
- `windows/` — Windows diagnostic notes and report.
- `linux/` — Linux diagnostic notes and report.
- `evidence/` — Sanitized screenshots supporting the test records.
- `reports/` — Final troubleshooting reports.

## Skills Practised

- Windows 11 diagnostics
- Linux system diagnostics
- Command-line troubleshooting
- Disk and memory inspection
- Networking fundamentals
- Technical documentation
- Evidence management

## Scope and Limitations

This project records basic diagnostic observations on personal systems. It is not a comprehensive hardware assessment, security audit, or proof of external network connectivity.

All published evidence should be reviewed and sanitized to avoid exposing sensitive information.

## Future Improvements

- Investigate common simulated troubleshooting scenarios.
- Document diagnostic reasoning and verified resolutions.
- Add a structured test log and troubleshooting procedures.
- Expand the documentation as further tests are completed.

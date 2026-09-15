# Ransomware Source Code - Defensive Analysis Only

> **WARNING:** This repository contains ransomware source code. It is malicious software. Do not compile, execute, distribute, or deploy it on any computer or network.

## Purpose

This project is retained only for authorized defensive security research, malware analysis, and education. It is not safe software, is not a legitimate online-business application, and must never be used to attack, lock, damage, or access systems without explicit permission.

## Why this is real malware

The program contains multiple capabilities associated with actual ransomware. The table below describes what the code attempts to do:

| Component | What the code attempts to do |
| --- | --- |
| `AggressiveKillAllSecurity()` | Terminate Defender and antivirus processes and services |
| `BypassUAC()` | Attempt to weaken or bypass Windows UAC |
| `BypassSmartScreen()` | Attempt to disable SmartScreen |
| `BypassAMSI()` | Attempt to patch AMSI functions in memory |
| `AntiDebug()` | Detect debuggers and analysis tools |
| `AntiVM()` | Detect VirtualBox, VMware, and low-resource virtual machines |
| `HideProcess()` | Hide the window and attempt process concealment |
| `InstallPersistence()` | Create Run/RunOnce, scheduled-task, and service persistence |
| `EncryptAllDrives()` | Recursively encrypt files on fixed and removable drives |
| `NetworkReplication()` | Attempt network propagation using administrator credentials |
| Telegram functions | Provide remote command-and-control through Telegram |
| `SelfDelete()` | Attempt to delete its executable |
| `WatchdogThread()` | Attempt to restart the process if it closes |
| `HandleWrongPassword()` | Shut down Windows after failed password attempts |

These capabilities can cause data loss, system compromise, and harm to other users. The source must be treated as real malware, even if it was created for learning or testing.

## Safety

- Do not run the source or any executable produced from it.
- Do not test it on a personal computer, shared host, or connected network.
- Do not provide it with administrator privileges.
- Treat the source as potentially malicious and scan it with trusted security tools.
- The previously embedded Telegram token and passwords have been redacted from this copy. Revoke the Telegram token through BotFather and rotate any credentials that appeared in older copies immediately.
- The source is deliberately blocked from compilation with a preprocessor error.

## Contents

- `Ransmware.c` - Ransomware source code retained for defensive analysis and deliberately disabled from compilation.

## Responsible handling

Use isolated, disposable malware-analysis infrastructure only, with appropriate authorization and network containment. For learning purposes, prefer benign toy examples that operate only on temporary test data and do not disable security controls, persist, spread, or contact external services.

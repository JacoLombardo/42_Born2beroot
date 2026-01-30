# Born2beroot

Born2beroot is a 42 School system administration project. The goal is to set up and secure a Linux virtual machine from scratch, focusing on virtualization, partitioning, security policies, and server management.

## Overview

Unlike most 42 projects centered on coding, this one immerses students in system administration and DevOps fundamentals. You create a secure VM using VirtualBox with strict security requirements—no graphical interface.

## Requirements

**System setup**

- Install Debian (recommended) or Rocky Linux
- Configure LVM partitioning with encrypted partitions
- Set up SSH on port 4242 with root login disabled
- Enable firewall (UFW or Firewalld)
- Ensure AppArmor or SELinux is active

**Security configuration**

- Create a user and add to `user42` and `sudo` groups
- Enforce strong password policies (10+ characters, 30-day expiry, mixed character types)
- Configure sudo with authentication limits, logging, and custom error messages
- Implement a monitoring script displaying system information every 10 minutes

## Composition

The project is organized around:

- **Subject**: `Born2beroot_subject.pdf` — full assignment specifications
- **Signature**: `signature.txt` — proof of completion for evaluation

## Technology

- VirtualBox
- Debian or Rocky Linux
- LVM, encryption (LUKS)
- SSH, UFW/Firewalld
- AppArmor/SELinux
- Bash scripting

## Setup

1. Install VirtualBox on your host machine
2. Create a new VM and install Debian or Rocky Linux (minimal, no GUI)
3. Follow the subject requirements for partitioning, LVM, and encryption
4. Configure SSH, firewall, sudo, and password policies
5. Create and run the monitoring script with `crontab`

## Notes

- No code repository; the deliverable is the configured VM and signature
- Security principles apply to cloud infrastructure, DevSecOps, and zero-trust architecture
- Required for 42 common core, typically part of the system administration track

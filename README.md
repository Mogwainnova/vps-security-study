# VPS Security & Performance Study (1GB RAM)

## Overview

This project explores the limits of a minimal VPS (1 vCPU, 1GB RAM) exposed to the Internet.

The goal was to answer a simple question:

👉 Can a low-cost VPS safely handle real-world traffic and attacks?

---

## Setup

- Nginx (web server)
- Cowrie (SSH honeypot)
- Fail2ban
- Encrypted backups (rclone + B2)

---

## Key Results

- 1,819,987 SSH events captured (39 days)
- 4,331 unique IPs
- 100% automated attacks (24/7)

Performance:
- ~330 requests/sec max
- 0 errors under load
- Main bottleneck: TLS, not CPU

---

## Security Insights

- Default credentials dominate attacks
- Brute-force is massive but unsophisticated
- Minimal hardening is effective

---

## Report

Full report available here:
👉 [rapport.pdf](./Rapport_technique_d_exploitation_d_infrastructure.pdf)

---

## Why this project matters

This study shows that:
- minimal infrastructure can be viable
- but requires careful trade-offs

---

## Author

Mogwainnova

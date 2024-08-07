---
header_title: "Implications"
header_menu: true
title: "Security Implications"
weight: 5
slug: "implications"
---

To the best of our knowledge, only the T-Head XuanTie C910 CPU in the TH1520 SoC is affected by GhostWrite. 
Still, this vulnerability impacts a wide range of devices, including personal computers, laptops, containers, and virtual machines in cloud servers. 
Therefore, any customers or vendors using machines with these processors are at risk.

Vulnerable devices include:
- [Scaleway Elastic Metal RV1](https://labs.scaleway.com/en/em-rv1/), bare-metal C910 cloud instances
- [Lichee Cluster 4A](https://sipeed.com/licheepi4a), compute cluster
- [Lichee Book 4A](https://sipeed.com/licheepi4a), laptop
- [Lichee Console 4A](https://sipeed.com/licheepi4a), tiny laptop
- [Lichee Pocket 4A](https://www.tomshardware.com/pc-components/cpus/risc-v-handheld-gaming-system-announced-linux-as-the-basis-for-a-retro-gaming-platform), gaming console
- [Sipeed Lichee Pi 4A](https://sipeed.com/licheepi4a), single-board computer (SBC)
- [Milk-V Meles](https://milkv.io/meles), SBC
- [BeagleV-Ahead](https://www.beagleboard.org/boards/beaglev-ahead), SBC

To protect against this vulnerability, you can disable the vulnerable vector extension entirely. 

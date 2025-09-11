---
author: Leon Trampert
title: "GhostWrite"
logo: "/ghostwrite.svg"
logo_header: "/ghostwrite-no-text.svg"
header_title: "Home"
header_menu: true
date: 07-10-2023
---

The GhostWrite vulnerability affects the T-Head XuanTie C910 and C920 RISC-V CPUs. 
This vulnerability allows unprivileged attackers, even those with limited access, to read and write any part of the computer's memory and to control peripheral devices like network cards. 
GhostWrite renders the CPU's security features ineffective and cannot be fixed without disabling around half of the CPU's functionality.

{{< linkbutton title="READ" icon="fas fa-book fa-1x" url="/riscover_ccs25.pdf" >}}

<div class="columns" style="margin-top: 1rem">
    <div>
{{< modalbutton title="CITE" icon="fa-solid fa-quote-left" id="citebutton" classes="buttonoutline buttonsmall" >}}
@inproceedings{Thomas2025Ghostwrite,
 author = {Fabian Thomas and Eric Garc{\'i}a Arribas and Lorenz Hetterich and Daniel Weber and Lukas Gerlach and Ruiyi Zhang and Michael Schwarz},
 booktitle = {CCS},
 title = {{RISCover: Automatic Discovery of User-exploitable Architectural Security Vulnerabilities in Closed-Source RISC-V CPUs}},
 year = {2025}
}
{{< /modalbutton >}}
    </div>
    <div>
{{< linkbutton title="TRY" icon="fas fa-flask fa-1x" url="https://github.com/cispa/ghostwrite" classes="buttonoutline buttonsmall" >}}
    </div>
</div>

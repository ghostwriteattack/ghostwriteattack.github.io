---
header_title: "How we found it"
header_menu: true
weight: 50
slug: "how-we-found-it"
---

{{< smallcolumn reverse=false >}}
{{< icon src="/differential-fuzzing.svg" alt="An overview of differential CPU fuzzing." >}}
<--->

{{< title title="Automatic Bug Discovery." subtitle="Differential CPU Fuzz Testing.">}}


We discovered GhostWrite by analyzing both documented and undocumented instructions using a method called differential fuzz-testing for CPUs. 
The concept is intuitive: generate small programs, run them on different CPUs, and compare the results. 
Since every RISC-V CPU should follow the [RISC-V specification](https://riscv.org/technical/specifications/), they should produce the same results for the same inputs. 
When results differ between CPUs, it suggests that one of the CPUs might have an issue.

We identified GhostWrite when the T-Head XuanTie C910 CPU showed unusual behavior with an illegally-encoded vector-store instruction. 
While other CPUs generated page fault exceptions or refused to execute the instruction, the C910 did execute it.

Upon further investigation, we discovered that the illegally-encoded instruction allows a process to write directly to *physical* memory instead of *virtual* memory, revealing a severe security vulnerability.

{{< /smallcolumn >}}

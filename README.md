# 👋 Hi, I'm Jihoon Choi

I'm a Computer Science student at **UBC** currently looking for **co-op and internship opportunities**.

I got into programming through Arduino — watching hardware respond to code made me want to understand what was actually happening underneath, which pushed me toward low-level and systems work. But I've also built production web apps, and I enjoy both ends of the stack for different reasons.

Either way, I care more about understanding systems than collecting tools. When I hit a bug, I don't move on until I know exactly why it happened and why the fix works.

---

### Projects

**[T1_Hypervisor](https://github.com/JihoonChoi1/T1_Hypervisor)** — a Type 1 bare-metal hypervisor for ARMv8-A in `no_std` Rust, targeting QEMU `virt` and Raspberry Pi 4. Boots at EL2, brings up a Stage-1 MMU (W^X enforced), GICv2, and all four cores via PSCI, then constructs per-VM Stage-2 translation tables for two guests: a Management VM on core 0 (owns the UART and GIC) and an HFT engine VM on cores 1–3 (interrupt-masked at the hardware level, cache-colored pages to reduce L2 contention). Guest RAM is allocated, colored, zeroed, cleaned to PoC, and mapped at 4 KiB granularity; the HFT payload is loaded and `vcpu[0]` is seeded. VM entry is the next and final milestone.

**[MyOS](https://github.com/cjihoon/my-os)** — a 32-bit x86 operating system built from scratch in C, including a preemptive scheduler, virtual/physical memory manager, ELF loader, and ATA driver. The parts I enjoyed most were the ones that required understanding how the hardware and software contract actually works — interrupt handling, memory management, assembly-level debugging.

**[ATM Lab Website](https://github.com/JihoonChoi1/ATM-Lab-website)** — a full-stack academic website and CMS for Ajou University's Advanced Thermal Management Lab, built with Next.js 14 (App Router), Prisma, and PostgreSQL. Features a password-protected admin UI with full CRUD over all content, Tiptap rich-text editing, image upload with `sharp` thumbnail generation, TOTP 2FA, IP-based rate limiting, per-request CSP nonces, and an audit log. Deployed at [atm-lab-website.vercel.app](https://atm-lab-website.vercel.app) and on the lab's school server.

---

### Tech

**Languages:** C, C++, Rust, Python, TypeScript
**Tools:** Linux, QEMU, Git, Docker, Next.js, Prisma
**Interests:** Operating systems, ARM/x86 architecture, kernel development, virtualization

---

### Outside of code

Badminton, escape rooms, iced americanos, and too many YouTube rabbit holes.

📧 [cjihoon1234@gmail.com](mailto:cjihoon1234@gmail.com)
💼 [LinkedIn](https://www.linkedin.com/in/jihoon-choi-60a5b52a0/)

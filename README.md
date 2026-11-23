# Awesome-Security-Auditing-Container-Sandboxing

## Top Security Auditing & Container Sandboxing Ecosystem



**Curated List of SaaS/Hosted Platforms & Open-Source GitHub Projects**  

*Focused on Container Isolation, MicroVMs, Runtime Syscall Security, Vulnerability Scanning & Kernel Sandboxing*  

**Last updated: November 2026**



This repository tracks notable **SaaS/hosted cloud-native security platforms** and **open-source GitHub projects** for **Security Auditing & Container Sandboxing**. These tools isolate untrusted workloads (including AI code-execution agents and multi-tenant containers) using user-space kernels, lightweight MicroVMs, Linux namespaces/seccomp/Landlock sandboxes, eBPF runtime threat detection, and SBOM/CVE image scanners.



**Examples** include gabrielelozupone/kokon, gVisor, Firecracker, Kata Containers, Falco, Tetragon, Trivy, Grype, Syft, Bubblewrap, nsjail, Lynis, Aqua Security, Sysdig Secure, Prisma Cloud, Wiz, Docker Scout, and Snyk Container.



**Open-source emphasis**: This list heavily expands on active open-source container sandboxes, MicroVM hypervisors, eBPF runtime security monitors, Linux sandboxing primitives, and container vulnerability auditors — ideal for DevSecOps engineers, platform architects, security researchers, and AI sandbox builders.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saashosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Wiz](https://wiz.io)**  

  Cloud-native application protection platform (CNAPP) providing agentless container, Kubernetes, and cloud workload vulnerability scanning, runtime sensors, and attack-path analysis.



- **[Prisma Cloud (Palo Alto Networks)](https://paloaltonetworks.com)**  

  Enterprise CNAPP suite offering container image compliance auditing, runtime defense, Web Application and API Security (WAAS), and host/serverless protection.



- **[Aqua Security](https://aquasec.com)**  

  Cloud-native container and Kubernetes security platform providing image assurance, dynamic threat analysis, eBPF runtime enforcement, and supply-chain security.



- **[Sysdig Secure](https://sysdig.com)**  

  Cloud security and runtime threat detection platform built on Falco, delivering real-time container auditing, vulnerability management, and incident forensics.



- **[Docker Scout](https://docker.com)**  

  Hosted container supply-chain analysis and policy evaluation service integrated into Docker Hub and Docker Desktop for continuous CVE tracking and base-image remediation.



- **[Snyk Container](https://snyk.io)**  

  Developer-first container and Kubernetes security SaaS detecting OS package and application vulnerabilities in Dockerfiles and images with automated base-image upgrade advice.



- **[E2B (Code Interpreter Sandboxes)](https://e2b.dev)**  

  Cloud-hosted Firecracker MicroVM sandboxing API built specifically for isolating untrusted AI agent code execution and browser sessions.



- **[Fly.io Machines (Firecracker Cloud)](https://fly.io)**  

  Edge application platform running user containers inside isolated Firecracker MicroVMs with fast cold starts and hardware-virtualized multi-tenancy.





## Open-Source GitHub Projects



- **[Kokon (gabrielelozupone/kokon)](https://github.com)**  

  Open-source lightweight container sandboxing and security auditing utility designed for isolated execution environments and fine-grained workload containment.



- **[gVisor (google/gVisor)](https://github.com)**  

  Application kernel written in Go that implements a substantial portion of the Linux system interface in userspace, providing strong OCI container isolation (`runsc`) without VM overhead.



- **[Firecracker (firecracker-microvm/firecracker)](https://github.com)**  

  Open-source Virtual Machine Monitor (VMM) written in Rust using Linux KVM to create and manage secure, multi-tenant MicroVMs with minimal memory footprint and sub-second startup.



- **[Kata Containers (kata-containers/kata-containers)](https://github.com)**  

  Open-source container runtime that builds lightweight virtual machines feeling and performing like standard containers while providing hardware-isolated kernel boundaries.



- **[Falco (falcosecurity/falco)](https://github.com)**  

  CNCF graduated open-source cloud-native runtime security engine using eBPF and kernel probes to detect anomalous container syscalls, shell spawns, and privilege escalations in real time.



- **[Cilium Tetragon (cilium/tetragon)](https://github.com)**  

  eBPF-based security observability and runtime enforcement tool capable of detecting and synchronously blocking malicious syscalls, file accesses, and network sockets inside the Linux kernel.



- **[Trivy (aquasecurity/trivy)](https://github.com)**  

  Comprehensive open-source vulnerability, misconfiguration, secret, and SBOM scanner for container images, filesystems, Git repositories, and Kubernetes clusters.



- **[Grype (anchore/grype)](https://github.com)** & **[Syft (anchore/syft)](https://github.com)**  

  Open-source CLI tools by Anchore for generating Software Bills of Materials (SBOMs) from container images (`Syft`) and matching them against vulnerability databases (`Grype`).



- **[Bubblewrap (`bwrap`) (containers/bubblewrap)](https://github.com)**  

  Low-level, unprivileged sandboxing tool for Linux utilizing user namespaces, mount namespaces, and seccomp filters (powering Flatpak and local AI sandboxes).



- **[nsjail (google/nsjail)](https://github.com)**  

  Lightweight process isolation tool by Google combining Linux namespaces, cgroups, `rlimits`, and `kafel` seccomp-bpf syscall policies for sandboxing untrusted binaries.



- **[Lynis (CISOfy/lynis)](https://github.com)**  

  Battle-tested open-source security auditing and compliance hardening tool for Linux, macOS, and Unix host systems running container workloads.



- **[Docker Bench for Security (docker/docker-bench-security)](https://github.com)** & **[kube-bench (aquasecurity/kube-bench)](https://github.com)**  

  Open-source auditing scripts that check Docker daemons and Kubernetes deployments against official CIS Security Benchmarks.



- **[Sysbox (nestybox/sysbox)](https://github.com)**  

  Open-source OCI container runtime ("runc on steroids") enabling rootless Docker-in-Docker and Kubernetes-in-Docker sandboxes using Linux user-namespace isolation.



### Additional Strong Open-Source Options



- **[Firejail (netblue30/firejail)](https://github.com)** — SUID sandbox program reducing the risk of security breaches by restricting the running environment of untrusted Linux applications via seccomp-bpf and namespaces.

- **[Youki (youki-dev/youki)](https://github.com)** & **[crun (containers/crun)](https://github.com)** — High-speed open-source OCI container runtimes written in Rust and C with native `seccomp`, `Landlock`, and rootless cgroup v2 support.

- **[Kubescape (kubescape/kubescape)](https://github.com)** — CNCF open-source Kubernetes security platform offering NSA/MITRE posture auditing, RBAC visualization, and eBPF runtime reachability analysis.

- **[Clair (quay/clair)](https://github.com)** — Open-source static vulnerability analysis engine designed for container registries (Quay, Harbor).

- **[Tracee (aquasecurity/tracee)](https://github.com)** — Linux runtime security and forensics tool leveraging eBPF to trace container system calls and behavioral signatures.

- **[Landlock / `landrun` (Zouuup/landrun)](https://github.com)** — Lightweight Go CLI wrapper leveraging the Linux Landlock LSM to sandbox arbitrary commands with strict filesystem and TCP port allowlists without root.

- **[srt — Sandbox Runtime (anthropic-experimental/sandbox-runtime)](https://github.com)** — Open-source OS-level sandboxing wrapper (`bubblewrap` on Linux, `sandbox-exec` on macOS) built to isolate terminal commands and AI coding agents.



**Frameworks for building custom systems**: Combine **Trivy** + **Syft** in CI/CD for pre-deployment image auditing, run untrusted multi-tenant or AI workloads inside **gVisor**, **Firecracker**, or **Bubblewrap**, and monitor production syscalls in real time with **Falco** or **Tetragon**.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Container sandboxing and kernel isolation mechanisms (`namespaces`, `seccomp`, `gVisor`, `Firecracker`) vary significantly in attack surface and kernel requirements; defense-in-depth (least privilege, read-only root filesystems, network egress policies, and non-root users) is always recommended.

- Security auditing tools (`Lynis`, `docker-bench-security`, `Falco`) should only be run on hosts, clusters, and container registries you own or have explicit authorization to audit.



---



**Made for DevSecOps engineers, security researchers, platform architects, and open-source builders.**  

Let's make security auditing and container sandboxing verifiable, resilient, and open to everyone.

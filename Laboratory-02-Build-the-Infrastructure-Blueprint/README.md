# Laboratory 02 – Build the Cloud Infrastructure Blueprint

## Mission Overview

This lab is about understanding the basics of cloud infrastructure before
actually deploying anything. Using a Linux server provided through the
KillerCoda Playground, this activity involved investigating the server's
specs, identifying the main infrastructure components (compute, storage,
networking, OS), comparing how AWS, Azure, and GCP offer similar
services, and putting together a simple cloud architecture diagram for a
fictional company — all as if preparing
documentation for a real client before a cloud deployment.

---

## Objectives

- Explain the major components of cloud infrastructure.
- Investigate the hardware and software resources available in a Linux
  environment.
- Differentiate compute, storage, networking, and identity resources.
- Interpret how cloud infrastructure components relate to each other.
- Create professional technical documentation using Markdown.
- Continue building a structured GitHub Cloud Computing Portfolio.

---

## Cloud Infrastructure Components

| Component | Found In This Lab |
|---|---|
| Compute | 1 vCPU (Intel Xeon E312xx) — checked with `lscpu`/`nproc` |
| Storage | 19G disk (`/dev/vda1`) — checked with `df -h` |
| Networking | IP addresses 172.30.1.2 / 172.17.0.1 — checked with `hostname -I` |
| Operating System | Ubuntu 24.04.4 LTS, kernel 6.8.0-138-generic |

More detail on each of these is documented in `cloud-components.md` and
`infrastructure-report.md`.

---

## Tools Used

- **KillerCoda Playground** – for accessing a live Linux server
- **Linux terminal commands** – for investigating system specs
- **Markdown** – for writing all documentation files
- **Diagramming tool** – for creating the cloud architecture diagram
- **GitHub** – for version control and submitting the portfolio

---

## Linux Commands Executed

| Command | Purpose |
|---|---|
| `cat /etc/os-release` | Check operating system info |
| `uname -r` | Check kernel version |
| `lscpu` | Check CPU model and core details |
| `nproc` | Check number of CPU cores |
| `free -h` | Check total RAM |
| `df -h` | Check disk capacity |
| `mount \| column -t` | Check mounted file systems |
| `hostname` | Check server hostname |
| `hostname -I` | Check IP address |

---

## Skills Learned

- How to check system specs (CPU, RAM, disk, OS) using Linux terminal
  commands.
- How to tell apart compute, storage, and networking resources in a real
  environment.
- How AWS, Azure, and GCP name their services differently even though
  they offer basically the same things.
- How to write clean technical documentation using Markdown (tables,
  headings, etc.).
- How to structure a GitHub repo/portfolio properly for a project.

---

## Challenges Encountered

- Some Linux commands (like `mount`) returned a lot of output, so it took
  extra effort to pick out only the relevant parts for documentation.
- Understanding how cloud provider services map to each other (e.g.,
  EC2 vs Virtual Machines vs Compute Engine) required doing outside
  research beyond just the terminal.

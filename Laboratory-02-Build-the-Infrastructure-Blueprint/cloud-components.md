# Cloud Infrastructure Components

This checkpoint identifies 4 main infrastructure components found in the
KillerCoda Linux environment: compute, storage, networking, and the
operating system.

---

## Compute Resources

This is basically the CPU of the server — the part that runs everything.
Checked using `lscpu` and `nproc`, which showed 1 CPU core (Intel Xeon
E312xx).

- **Purpose:** Processes instructions and runs the OS and apps.
- **Why it matters in cloud computing:** This is what's really being
  paid for when renting a cloud server. More CPU = more power, but also
  more cost.
- **In KillerCoda:** The instance was assigned 1 vCPU, kind of like how
  AWS gives a certain number of vCPUs when launching an EC2 instance.

---

## Storage Resources

This is where files and data are saved. Checked using `df -h`, showing
the main disk (`/dev/vda1`) has 19G total, with 13G still free.

- **Purpose:** Stores the OS, installed programs, and any data.
- **Why it matters in cloud computing:** Data needs to stay saved even
  if the server restarts. Cloud storage allows space to scale up
  without buying new hardware.
- **In KillerCoda:** The disk shown by `df -h` works like a storage
  volume attached to a VM, similar to an AWS EBS volume.

---

## Networking Resources

This lets the server connect to other systems and the internet. Checked
using `hostname -I`, which returned two IPs: 172.30.1.2 and 172.17.0.1.

- **Purpose:** Makes the server reachable so it can send/receive data.
- **Why it matters in cloud computing:** Without networking, no one
  could access whatever gets deployed. Cloud providers use virtual
  networks (like AWS VPC) to manage this.
- **In KillerCoda:** Having two IPs suggests the playground runs inside
  a container with its own internal network setup.

---

## Operating System

The OS manages everything running on the server. Checked using
`cat /etc/os-release`, which showed Ubuntu 24.04.4 LTS, kernel
6.8.0-138-generic.

- **Purpose:** Connects the hardware (CPU, RAM, disk) to the software
  running on top of it.
- **Why it matters in cloud computing:** Every cloud VM starts from an
  OS image. Picking the right OS affects what software can run.
- **In KillerCoda:** The playground comes pre-installed with Ubuntu,
  similar to picking a machine image when launching a cloud VM.
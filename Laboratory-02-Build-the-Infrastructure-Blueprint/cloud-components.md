# Cloud Infrastructure Components

## 1. Compute Resources

**What it is:** This is the CPU/processor of the server — the part that
actually runs programs and processes instructions. In the KillerCoda
environment, I checked this using `lscpu` and `nproc`, which showed
`[CPU model]` with `[X] core(s)`.

**Purpose:** It's the "brain" of the server. It handles all the processing
needed to run the OS and any applications on top of it.

**Why it's important in cloud computing:** Compute power is basically what
you're paying for when you rent a cloud server (like an EC2 instance in
AWS). More cores/CPU = more processing power, but also more cost, so
picking the right amount matters.

**Relation to KillerCoda:** KillerCoda gives us a temporary virtual machine
with a set amount of CPU, just like how a real cloud provider gives you a
compute instance when you launch one.

---

## 2. Storage Resources

**What it is:** This is where data is saved on the server. I used `df -h`
to check this, and it showed `[X]GB` of disk space across the mounted
filesystems.

**Purpose:** Storage keeps the OS files, installed programs, and any data
we create or save while using the server.

**Why it's important in cloud computing:** Cloud storage (like AWS S3 or
Azure Blob Storage) lets data stay saved even if the server itself is shut
down or restarted. It's a separate resource from compute because storage
needs are different — sometimes you need a lot of storage but not much
processing power, or the other way around.

**Relation to KillerCoda:** The disk space I saw with `df -h` is like the
storage volume attached to a cloud VM — similar to an EBS volume in AWS.

---

## 3. Networking Resources

**What it is:** This lets the server connect to other devices/the internet.
I checked the IP address using `hostname -I`, which showed `[IP address]`.

**Purpose:** Networking is what makes the server reachable — without it,
no one could access whatever is running on the server (like a website or
app).

**Why it's important in cloud computing:** Every cloud service needs
networking to actually be useful. Cloud providers set up virtual networks
(like AWS VPC or Azure VNet) so servers can talk to each other and to users
safely.

**Relation to KillerCoda:** The IP address given to my KillerCoda instance
works the same way — it's like the private IP a cloud provider assigns to
a VM inside its network.

---

## 4. Operating System

**What it is:** The OS manages everything on the server — hardware,
software, files, users. I checked this with `cat /etc/os-release`, which
showed `[OS name and version]`, running kernel `[kernel version]`.

**Purpose:** The OS is the middleman between the hardware (CPU, RAM, disk)
and the programs running on the server. It manages processes, files, and
permissions.

**Why it's important in cloud computing:** When you launch a cloud
instance, you always start from a base OS image. The OS you pick affects
what software you can install and how the server behaves, so it's one of
the first choices you make when setting up a cloud server.

**Relation to KillerCoda:** KillerCoda already comes pre-loaded with a
Linux OS, similar to how cloud providers let you pick a machine image
(like an AMI in AWS) when creating a new VM.
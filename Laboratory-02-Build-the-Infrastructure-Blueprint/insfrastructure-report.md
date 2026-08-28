# Infrastructure Report

## Operating System

| Attribute | Value |
|---|---|
| Name | Ubuntu |
| Version | 24.04.4 LTS (Noble Numbat) |
| ID | ubuntu |
| ID Like | debian |

Command used: `cat /etc/os-release`

---

## Kernel Version

| Attribute | Value |
|---|---|
| Kernel Version | 6.8.0-138-generic |

Command used: `uname -r`

---

## CPU Model

| Attribute | Value |
|---|---|
| Architecture | x86_64 |
| Model Name | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| Vendor | GenuineIntel |
| Virtualization | KVM (full virtualization) |
| L1d / L1i Cache | 32 KiB each |
| L2 Cache | 4 MiB |
| L3 Cache | 16 MiB |

Command used: `lscpu`

---

## Number of CPU Cores

| Attribute | Value |
|---|---|
| CPU(s) | 1 |
| Core(s) per socket | 1 |
| Thread(s) per core | 1 |
| Socket(s) | 1 |

Command used: `nproc` and `lscpu`

---

## Total RAM

| Type | Total | Used | Free | Available |
|---|---|---|---|---|
| Mem | 1.9 Gi | 414 Mi | 837 Mi | 1.5 Gi |
| Swap | 1.0 Gi | 0 B | 1.0 Gi | — |

Command used: `free -h`

---

## Disk Capacity

| Filesystem | Size | Used | Available | Use % | Mounted On |
|---|---|---|---|---|---|
| tmpfs | 191M | 996K | 190M | 1% | /run |
| /dev/vda1 | 19G | 5.4G | 13G | 30% | / |
| tmpfs | 952M | 84K | 952M | 1% | /dev/shm |
| tmpfs | 5.0M | 0 | 5.0M | 0% | /run/lock |
| /dev/vda16 | 881M | 117M | 703M | 15% | /boot |
| /dev/vda15 | 105M | 6.2M | 99M | 6% | /boot/efi |

Command used: `df -h`

---

## Mounted File Systems

| Device / Source | Mount Point | Type |
|---|---|---|
| /dev/vda1 | / | ext4 |
| /dev/vda16 | /boot | ext4 |
| /dev/vda15 | /boot/efi | vfat |
| tmpfs | /dev/shm | tmpfs |
| tmpfs | /run | tmpfs |
| tmpfs | /run/lock | tmpfs |
| proc | /proc | proc |
| sysfs | /sys | sysfs |
| udev | /dev | devtmpfs |
| cgroup2 | /sys/fs/cgroup | cgroup2 |
| securityfs | /sys/kernel/security | securityfs |
| debugfs | /sys/kernel/debug | debugfs |

Command used: `mount | column -t`


---

## Hostname

| Attribute | Value |
|---|---|
| Hostname | ubuntu |

Command used: `hostname`

---

## IP Address

| Attribute | Value |
|---|---|
| IP Address(es) | 172.30.1.2, 172.17.0.1 |

Command used: `hostname -I`

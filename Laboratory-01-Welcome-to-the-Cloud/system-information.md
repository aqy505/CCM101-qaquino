**Linux Distribution** 

&#x20;**(cat /etc/os-release)**

PRETTY\_NAME="Ubuntu 24.04.4 LTS"

NAME="Ubuntu"

VERSION\_ID="24.04"

VERSION="24.04.4 LTS (Noble Numbat)"

VERSION\_CODENAME=noble

ID=ubuntu

ID\_LIKE=debian

HOME\_URL="https://www.ubuntu.com/"

SUPPORT\_URL="https://help.ubuntu.com/"

BUG\_REPORT\_URL="https://bugs. launchpad.net/ubuntu/"

PRIVACY\_POLICY\_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"

JBUNTU\_CODENAME=noble

LOGO=ubuntu-logo





**Kernel Version** 

&#x20;**(uname -r)**

6.8.0-136-generic





**CPU Information** 

&#x20;**(lscpu)**

Architecture:                x86\_64

&#x20; CPU op-mode(s):            32-bit, 64-bit

&#x20; Address sizes:             39 bits physical, 48 bits virtual

&#x20; Byte Order:                Little Endian

CPU(s):                      1

&#x20; On-line CPU(s) list:       0

Vendor ID:                   GenuineIntel

&#x20; Model name:                Intel Xeon E312xx (Sandy Bridge, IBRS update)

&#x20;   CPU family:              6

&#x20;   Model:                   42

&#x20;   Thread(s) per core:      1

&#x20;   Core(s) per socket:      1

&#x20;   Socket(s):               1

&#x20;   Stepping:                1

&#x20;   BogoMIPS:                7008.00

&#x20;   Flags:                   fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 syscall nx rdtscp lm constant\_tsc rep\_go

&#x20;                            od nopl xtopology cpuid tsc\_known\_freq pni pclmulqdq ssse3 cx16 pcid sse4\_1 sse4\_2 x2apic popcnt tsc\_deadline\_timer aes xsave avx hypervis

&#x20;                            or lahf\_lm cpuid\_fault pti ssbd ibrs ibpb stibp tsc\_adjust xsaveopt arat md\_clear

Virtualization features:     

&#x20; Hypervisor vendor:         KVM

&#x20; Virtualization type:       full

Caches (sum of all):         

&#x20; L1d:                       32 KiB (1 instance)

&#x20; L1i:                       32 KiB (1 instance)

&#x20; L2:                        4 MiB (1 instance)

&#x20; L3:                        16 MiB (1 instance)

NUMA:                        

&#x20; NUMA node(s):              1

&#x20; NUMA node0 CPU(s):         0

Vulnerabilities:             

&#x20; Gather data sampling:      Not affected

&#x20; Indirect target selection: Mitigation; Aligned branch/return thunks

&#x20; Itlb multihit:             KVM: Mitigation: VMX unsupported

&#x20; L1tf:                      Mitigation; PTE Inversion

&#x20; Mds:                       Mitigation; Clear CPU buffers; SMT Host state unknown

&#x20; Meltdown:                  Mitigation; PTI

&#x20; Mmio stale data:           Unknown: No mitigations

&#x20; Reg file data sampling:    Not affected

&#x20; Retbleed:                  Not affected

&#x20; Spec rstack overflow:      Not affected

&#x20; Spec store bypass:         Mitigation; Speculative Store Bypass disabled via prctl

&#x20; Spectre v1:                Mitigation; usercopy/swapgs barriers and \_\_user pointer sanitization

&#x20; Spectre v2:                Mitigation; Retpolines; IBPB conditional; IBRS\_FW; STIBP disabled; RSB filling; PBRSB-eIBRS Not affected; BHI Retpoline

&#x20; Srbds:                     Not affected

&#x20; Tsa:                       Not affected

&#x20; Tsx async abort:           Not affected

&#x20; Vmscape:                   Not affected





**Total Memory**  

&#x20;**(free -h)**

&#x20;              total        used        free      shared  buff/cache   available

Mem:           1.9Gi       426Mi       848Mi       1.1Mi       795Mi       1.4Gi

Swap:          1.0Gi          0B       1.0Gi





**Available Disk Space** 

&#x20;**(df -h)**

Filesystem      Size  Used Avail Use% Mounted on

tmpfs           191M 1012K  190M   1% /run

/dev/vda1        19G  5.4G   13G  30% /

tmpfs           952M   84K  952M   1% /dev/shm

tmpfs           5.0M     0  5.0M   0% /run/lock

/dev/vda16      881M  117M  703M  15% /boot

/dev/vda15      105M  6.2M   99M   6% /boot/efi

tmpfs           191M  8.0K  191M   1% /run/user/1001


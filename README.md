# Nvidia Tesla K80 Gaming Guide
Use Nvidia Telsa K80 for Gaming in Windows 10 and Windows Server 2019.

Tested:
Windows 10 (21H1)
Windows Server 2019 (v1809)

==============================================================================

Step 1: Inteall Nvidia Tesla Driver (471.41-data-center-tesla-desktop-winserver-2019-2016-international.exe)
Step 2: Add Path for nvidia-smi (C:\Program Files\NVIDIA Corporation\NVSMI) and Reboot.
Step 3: Change to WDDM mode by Open Command prompt (run as administrator) and execute "nvidia-smi -g 0 -dm 0"
Step 4: Reboot and Enjoy!
Step 4b: Disable ECC for GPU 0 - Open Command prompt (run as administrator) and execute "nvidia-smi -g 0 -e 0"
Step 4c: Reboot.

-g 0  <= "0" mean gpu id, Tesla K80 have 2 GPU, 1 and 0

To Change back to TCC Mode:
Open Command prompt (run as administrator) and execute "nvidia-smi -g 0 -dm 1"

To Enable ECC:
Open Command prompt (run as administrator) and execute "nvidia-smi -g 0 -e 1"

To List GPU info:
Open Command prompt (run as administrator) and execute "nvidia-smi"

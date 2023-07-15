# VmMacOS
How setup macOs on a VirtualBox


Use this command to change to your VirtualBox installation directory.

cd "C:\Program Files\Oracle\VirtualBox\"

VBoxManage.exe modifyvm "name VM" --cpuidset 00000001 000106e5 00100800 0098e3fd bfebfbff
VBoxManage setextradata "name VM" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "iMac19,1"
VBoxManage setextradata "name VM" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"
VBoxManage setextradata "name VM" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Mac-AA95B1DDAB278B95"
VBoxManage setextradata "name VM" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"
VBoxManage setextradata "name VM" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 1

VBoxManage.exe setextradata “name VM” “VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC” 0

enable USB 3.0


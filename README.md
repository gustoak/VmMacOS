# VmMacOS
How setup macOs on a VirtualBox

MacOs ( IMG ) 
https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbGVMb2JQdTJLMk82RDlOTk9UVi0tLTk2SGlZZ3xBQ3Jtc0ttWTFRUm05VHZNNUhvc3RDY2ozSlBLM3JoUGJZQ19oZWFrTmdTc0pzb0xMTUZBazdvb3RvUW9DTDdDV3ZaUjc2M2dUZXliQUhqZGJpNTZoOEN3NGo4eXhmOE84dWdsTE9ka3JDaXdaZ3U2c3loLTlpRQ&q=https%3A%2F%2Fwww.mediafire.com%2Ffile%2F4fcx0aeoehmbnmp%2FmacOS%2BMonterey%2Bby%2BTechrechard.com.iso%2Ffile&v=Lq8J-vFqH7w

Use this command to change to your VirtualBox installation directory.

cd "C:\Program Files\Oracle\VirtualBox"


Replace Your VM Name with the name of your virtual machine and run all of the following commands on your host.

VBoxManage.exe modifyvm "Your VM Name" --cpuidset 00000001 000306a9 04100800 7fbae3ff bfebfbff

VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "MacBookPro11,3"

VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"

VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Mac-2BD1B31983FE1663"

VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"

VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 1


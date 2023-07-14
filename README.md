# VmMacOS
How setup macOs on a VirtualBox

MacOs ( IMG ) 
https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbGVMb2JQdTJLMk82RDlOTk9UVi0tLTk2SGlZZ3xBQ3Jtc0ttWTFRUm05VHZNNUhvc3RDY2ozSlBLM3JoUGJZQ19oZWFrTmdTc0pzb0xMTUZBazdvb3RvUW9DTDdDV3ZaUjc2M2dUZXliQUhqZGJpNTZoOEN3NGo4eXhmOE84dWdsTE9ka3JDaXdaZ3U2c3loLTlpRQ&q=https%3A%2F%2Fwww.mediafire.com%2Ffile%2F4fcx0aeoehmbnmp%2FmacOS%2BMonterey%2Bby%2BTechrechard.com.iso%2Ffile&v=Lq8J-vFqH7w

Use this command to change to your VirtualBox installation directory.

cd "C:\Program Files\Oracle\VirtualBox\"

VBoxManage.exe modifyvm "mcOS" --cpuidset 00000001 000106e5 00100800 0098e3fd bfebfbff

VBoxManage setextradata "mcOS" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "iMac19,1"

VBoxManage setextradata "mcOS" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"

VBoxManage setextradata "mcOS" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Mac-AA95B1DDAB278B95"

VBoxManage setextradata "mcOS" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"

VBoxManage setextradata "mcOS" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 1

VBoxManage setextradata "mcOS" VBoxInternal2/EfiGraphicsResolution 1920x1080


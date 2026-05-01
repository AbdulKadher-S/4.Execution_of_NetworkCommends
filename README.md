# 4.Execution_of_NetworkCommands
## AIM :Use of Network commands in Real Time environment
## Software : Command Prompt And Network Protocol Analyzer
## Procedure: To do this EXPERIMENT- follows these steps:
<BR>
In this EXPERIMENT- students have to understand basic networking commands e.g cpdump, netstat, ifconfig, nslookup ,traceroute and also Capture ping and traceroute PDUs using a network protocol analyzer 
<BR>
All commands related to Network configuration which includes how to switch to privilege mode
<BR>
and normal mode and how to configure router interface and how to save this configuration to
<BR>
flash memory or permanent memory.
<BR>
This commands includes
<BR>
• Configuring the Router commands
<BR>
• General Commands to configure network
<BR>
• Privileged Mode commands of a router 
<BR>
• Router Processes & Statistics
<BR>
• IP Commands
<BR>
• Other IP Commands e.g. show ip route etc.
<BR>

## Output
## 1.IPCONFIG
```bash
Microsoft Windows [Version 10.0.26200.8246]
(c) Microsoft Corporation. All rights reserved.

C:\Users\acer>ipconfig

Windows IP Configuration


Wireless LAN adapter Local Area Connection* 1:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Local Area Connection* 2:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Wi-Fi:

   Connection-specific DNS Suffix  . :
   IPv6 Address. . . . . . . . . . . : 2403:8600:c090:51:cd77:36ee:9d57:3ca3
   Temporary IPv6 Address. . . . . . : 2403:8600:c090:51:358e:ee11:5fe2:bd54
   Link-local IPv6 Address . . . . . : fe80::ebb3:ecd3:4342:36a%3
   Autoconfiguration IPv4 Address. . : 169.254.197.8
   Subnet Mask . . . . . . . . . . . : 255.255.0.0
   Default Gateway . . . . . . . . . : fe80::eedd:24ff:fe3d:ced5%3

Ethernet adapter Ethernet:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :
```
```
C:\Users\acer>hostname
Abdul-PC
```
```
C:\Users\acer>tracert

Usage: tracert [-d] [-h maximum_hops] [-j host-list] [-w timeout]
               [-R] [-S srcaddr] [-4] [-6] target_name

Options:
    -d                 Do not resolve addresses to hostnames.
    -h maximum_hops    Maximum number of hops to search for target.
    -j host-list       Loose source route along host-list (IPv4-only).
    -w timeout         Wait timeout milliseconds for each reply.
    -R                 Trace round-trip path (IPv6-only).
    -S srcaddr         Source address to use (IPv6-only).
    -4                 Force using IPv4.
    -6                 Force using IPv6.

C:\Users\acer>ping www.google.com

Pinging www.google.com [2001:4860:482b:7700::] with 32 bytes of data:
Reply from 2001:4860:482b:7700::: time=76ms
Reply from 2001:4860:482b:7700::: time=13ms
Reply from 2001:4860:482b:7700::: time=14ms
Reply from 2001:4860:482b:7700::: time=38ms

Ping statistics for 2001:4860:482b:7700:::
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 13ms, Maximum = 76ms, Average = 35ms
```
```
C:\Users\acer>netstat

Active Connections

  Proto  Local Address          Foreign Address        State
  TCP    127.0.0.1:5141         Abdul-PC:64823         ESTABLISHED
  TCP    127.0.0.1:46935        Abdul-PC:56758         ESTABLISHED
  TCP    127.0.0.1:46936        Abdul-PC:49684         ESTABLISHED
  TCP    127.0.0.1:46937        Abdul-PC:49686         ESTABLISHED
  TCP    127.0.0.1:49669        Abdul-PC:49670         ESTABLISHED
  TCP    127.0.0.1:49670        Abdul-PC:49669         ESTABLISHED
  TCP    127.0.0.1:49674        Abdul-PC:49675         ESTABLISHED
  TCP    127.0.0.1:49675        Abdul-PC:49674         ESTABLISHED
  TCP    127.0.0.1:49677        Abdul-PC:49678         ESTABLISHED
  TCP    127.0.0.1:49678        Abdul-PC:49677         ESTABLISHED
  TCP    127.0.0.1:49679        Abdul-PC:49680         ESTABLISHED
  TCP    127.0.0.1:49680        Abdul-PC:49679         ESTABLISHED
  TCP    127.0.0.1:49681        Abdul-PC:49682         ESTABLISHED
  TCP    127.0.0.1:49682        Abdul-PC:49681         ESTABLISHED
  TCP    127.0.0.1:49683        Abdul-PC:49685         ESTABLISHED
  TCP    127.0.0.1:49684        Abdul-PC:46936         ESTABLISHED
  TCP    127.0.0.1:49685        Abdul-PC:49683         ESTABLISHED
  TCP    127.0.0.1:49686        Abdul-PC:46937         ESTABLISHED
  TCP    127.0.0.1:52466        Abdul-PC:58995         ESTABLISHED
  TCP    127.0.0.1:56752        Abdul-PC:56753         ESTABLISHED
  TCP    127.0.0.1:56753        Abdul-PC:56752         ESTABLISHED
  TCP    127.0.0.1:56754        Abdul-PC:56755         ESTABLISHED
  TCP    127.0.0.1:56755        Abdul-PC:56754         ESTABLISHED
  TCP    127.0.0.1:56756        Abdul-PC:56757         ESTABLISHED
  TCP    127.0.0.1:56757        Abdul-PC:56756         ESTABLISHED
  TCP    127.0.0.1:56758        Abdul-PC:46935         ESTABLISHED
  TCP    127.0.0.1:58995        Abdul-PC:52466         ESTABLISHED
  TCP    127.0.0.1:58995        Abdul-PC:63333         ESTABLISHED
  TCP    127.0.0.1:58995        Abdul-PC:63345         ESTABLISHED
  TCP    127.0.0.1:63333        Abdul-PC:58995         ESTABLISHED
  TCP    127.0.0.1:63345        Abdul-PC:58995         ESTABLISHED
  TCP    127.0.0.1:64823        Abdul-PC:5141          ESTABLISHED
  TCP    [::1]:15161            Abdul-PC:50737         ESTABLISHED
  TCP    [::1]:15161            Abdul-PC:61420         TIME_WAIT
  TCP    [::1]:15161            Abdul-PC:63334         ESTABLISHED
  TCP    [::1]:50737            Abdul-PC:15161         ESTABLISHED
  TCP    [::1]:61421            Abdul-PC:15161         TIME_WAIT
  TCP    [::1]:63334            Abdul-PC:15161         ESTABLISHED
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:49411  [2603:1040:a06:6::1]:https  ESTABLISHED
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:50731  [2603:1040:a06:6::1]:https  ESTABLISHED
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:51205  [2606:50c0:8000::154]:https  ESTABLISHED
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:54186  sg-in-f188:5228        ESTABLISHED
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:57365  lb-140-82-112-22-iad:https  ESTABLISHED
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:58567  62:https               ESTABLISHED
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:58992  [64:ff9b::34b6:8fd2]:https  ESTABLISHED
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:59924  [2403:8600:80c0:4a::e62:100a]:https  ESTABLISHED
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:60500  [64:ff9b::acbc:9b19]:https  ESTABLISHED
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:61418  [64:ff9b::14be:9224]:https  TIME_WAIT
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:61419  [64:ff9b::285a:899]:https  TIME_WAIT
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:61735  cdn-185-199-110-133:https  ESTABLISHED
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:62723  whatsapp-cdn6-shv-03-maa3:5222  ESTABLISHED
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:62757  lb-140-82-112-26-iad:https  ESTABLISHED
  TCP    [2403:8600:c090:51:358e:ee11:5fe2:bd54]:63242  [64:ff9b::2d8e:e92]:https  ESTABLISHED
```
```
C:\Users\acer>systeminfo

Host Name:                     ABDUL-PC
OS Name:                       Microsoft Windows 11 Home Single Language
OS Version:                    10.0.26200 N/A Build 26200
OS Manufacturer:               Microsoft Corporation
OS Configuration:              Standalone Workstation
OS Build Type:                 Multiprocessor Free
Registered Owner:              acer
Registered Organization:       N/A
Product ID:                    00342-42784-66158-AAOEM
Original Install Date:         01-09-2025, 15:21:05
System Boot Time:              01-05-2026, 20:57:22
System Manufacturer:           Acer
System Model:                  TravelMate P215-75-G2-TCO
System Type:                   x64-based PC
Processor(s):                  1 Processor(s) Installed.
                               [01]: Intel64 Family 6 Model 170 Stepping 4 GenuineIntel ~1200 Mhz
BIOS Version:                  INSYDE Corp. V1.05tt01a, 01-09-2025
Windows Directory:             C:\Windows
System Directory:              C:\Windows\system32
Boot Device:                   \Device\HarddiskVolume1
System Locale:                 en-us;English (United States)
Input Locale:                  00004009
Time Zone:                     (UTC+05:30) Chennai, Kolkata, Mumbai, New Delhi
Total Physical Memory:         15,869 MB
Available Physical Memory:     6,598 MB
Virtual Memory: Max Size:      18,301 MB
Virtual Memory: Available:     7,135 MB
Virtual Memory: In Use:        11,166 MB
Page File Location(s):         C:\pagefile.sys
Domain:                        WORKGROUP
Logon Server:                  \\ABDUL-PC
Hotfix(s):                     5 Hotfix(s) Installed.
                               [01]: KB5082417
                               [02]: KB5054156
                               [03]: KB5083769
                               [04]: KB5083532
                               [05]: KB5088467
Network Card(s):               2 NIC(s) Installed.
                               [01]: Intel(R) Wi-Fi 6E AX211 160MHz
                                     Connection Name: Wi-Fi
                                     DHCP Enabled:    Yes
                                     DHCP Server:     255.255.255.255
                                     IP address(es)
                                     [01]: 169.254.197.8
                                     [02]: fe80::ebb3:ecd3:4342:36a
                                     [03]: 2403:8600:c090:51:358e:ee11:5fe2:bd54
                                     [04]: 2403:8600:c090:51:cd77:36ee:9d57:3ca3
                               [02]: Realtek PCIe GbE Family Controller
                                     Connection Name: Ethernet
                                     Status:          Media disconnected
Virtualization-based security: Status: Running
                               Required Security Properties:
                                     Base Virtualization Support
                               Available Security Properties:
                                     Base Virtualization Support
                                     Secure Boot
                                     DMA Protection
                                     UEFI Code Readonly
                                     SMM Security Mitigations 1.0
                                     Mode Based Execution Control
                                     APIC Virtualization
                               Services Configured:
                                     Hypervisor enforced Code Integrity
                               Services Running:
                                     Hypervisor enforced Code Integrity
                               App Control for Business policy: Enforced
                               App Control for Business user mode policy: Off
                               Security Features Enabled:
Hyper-V Requirements:          A hypervisor has been detected. Features required for Hyper-V will not be displayed.
```
```
C:\Users\acer>getmac

Physical Address    Transport Name
=================== ==========================================================
FC-6D-77-6D-9C-46   \Device\Tcpip_{05DFA269-CEFB-4295-ADCE-7123750CCF35}
74-D4-DD-CF-7A-F3   Media disconnected
```
```
C:\Users\acer>tasklist

Image Name                     PID Session Name        Session#    Mem Usage
========================= ======== ================ =========== ============
System Idle Process              0 Services                   0          8 K
System                           4 Services                   0        148 K
Secure System                  260 Services                   0     63,076 K
Registry                       304 Services                   0     63,188 K
smss.exe                       828 Services                   0      1,424 K
csrss.exe                     1220 Services                   0      6,564 K
wininit.exe                   1324 Services                   0      8,424 K
csrss.exe                     1332 Console                    1      7,476 K
winlogon.exe                  1420 Console                    1     16,512 K
services.exe                  1440 Services                   0     19,208 K
LsaIso.exe                    1488 Services                   0      4,148 K
lsass.exe                     1496 Services                   0     29,960 K
svchost.exe                   1624 Services                   0     40,780 K
fontdrvhost.exe               1656 Console                    1      4,412 K
fontdrvhost.exe               1664 Services                   0      3,804 K
WUDFHost.exe                  1700 Services                   0      9,932 K
svchost.exe                   1792 Services                   0     19,256 K
svchost.exe                   1852 Services                   0     13,332 K
WUDFHost.exe                  1928 Services                   0     21,624 K
dwm.exe                       1992 Console                    1   3,79,160 K
svchost.exe                    800 Services                   0      6,268 K
svchost.exe                   1316 Services                   0     10,972 K
svchost.exe                   2096 Services                   0     11,632 K
svchost.exe                   2144 Services                   0     15,096 K
svchost.exe                   2152 Services                   0     13,408 K
svchost.exe                   2160 Services                   0      7,684 K
svchost.exe                   2168 Services                   0     16,600 K
svchost.exe                   2208 Services                   0     10,328 K
svchost.exe                   2316 Services                   0     11,500 K
svchost.exe                   2364 Services                   0      7,032 K
svchost.exe                   2372 Services                   0     13,428 K
svchost.exe                   2428 Services                   0      9,736 K
svchost.exe                   2468 Services                   0     21,880 K
WUDFHost.exe                  2496 Services                   0     21,368 K
svchost.exe                   2668 Services                   0     22,072 K
svchost.exe                   2776 Services                   0     14,048 K
svchost.exe                   3128 Services                   0     10,604 K
svchost.exe                   3268 Services                   0     19,904 K
svchost.exe                   3296 Services                   0     19,280 K
svchost.exe                   3304 Services                   0     10,340 K
svchost.exe                   3312 Services                   0      7,564 K
Memory Compression            3416 Services                   0   3,44,752 K
svchost.exe                   3456 Services                   0     11,476 K
svchost.exe                   3508 Services                   0      9,656 K
svchost.exe                   3516 Services                   0     11,308 K
svchost.exe                   3524 Services                   0      8,860 K
svchost.exe                   3648 Services                   0     18,960 K
svchost.exe                   3700 Services                   0     10,872 K
svchost.exe                   3848 Services                   0     25,220 K
svchost.exe                   3904 Services                   0     12,620 K
audiodg.exe                   3972 Services                   0     26,172 K
svchost.exe                   4020 Services                   0     24,396 K
svchost.exe                   4048 Services                   0     18,740 K
spoolsv.exe                   3156 Services                   0     19,736 K
svchost.exe                   3196 Services                   0     24,792 K
svchost.exe                   1392 Services                   0     10,348 K
svchost.exe                   3964 Services                   0     22,232 K
AAADSvc.exe                   4228 Services                   0      7,372 K
ARTAimmxService.exe           4220 Services                   0      7,444 K
ADESv2Svc.exe                 4240 Services                   0      8,328 K
AcerCCAgent.exe               4248 Services                   0     23,816 K
AcerPixyService.exe           4260 Services                   0     16,276 K
AICO2_svc.exe                 4272 Services                   0      9,200 K
AcerGAICameraService.exe      4280 Services                   0      8,488 K
AICO_svc.exe                  4288 Services                   0      9,744 K
AcerEZService.exe             4296 Services                   0     20,972 K
AcerQAAgent.exe               4304 Services                   0     49,672 K
AcerSystemCentralService.     4312 Services                   0      7,636 K
AcerServiceWrapper.exe        4320 Services                   0     20,236 K
FMService64.exe               4332 Services                   0     18,632 K
svchost.exe                   4340 Services                   0     12,236 K
AcerDIAgent.exe               4348 Services                   0     23,712 K
GameInputRedistService.ex     4356 Services                   0     12,852 K
svchost.exe                   4364 Services                   0     62,872 K
svchost.exe                   4372 Services                   0     10,128 K
DtsApo4Service.exe            4380 Services                   0     21,628 K
svchost.exe                   4400 Services                   0     37,536 K
OfficeClickToRun.exe          4416 Services                   0     55,564 K
ipfsvc.exe                    4424 Services                   0      9,496 K
IntelAudioService.exe         4460 Services                   0     30,852 K
svchost.exe                   4728 Services                   0     15,400 K
ipf_uf.exe                    4748 Services                   0      9,296 K
jtagserver.exe                4760 Services                   0      6,080 K
MpDefenderCoreService.exe     4784 Services                   0     31,148 K
MorphoPixyService.exe         4800 Services                   0     18,488 K
SafeExamBrowser.Service.e     4916 Services                   0     28,160 K
RstMwService.exe              4924 Services                   0     10,452 K
RtkAudUService64.exe          4968 Services                   0     26,500 K
svchost.exe                   5036 Services                   0     12,904 K
svchost.exe                   5048 Services                   0      7,404 K
WMIRegistrationService.ex     5072 Services                   0     15,976 K
svchost.exe                   5080 Services                   0     27,712 K
svchost.exe                   5088 Services                   0     22,768 K
MsMpEng.exe                   5096 Services                   0   2,00,044 K
svchost.exe                   5540 Services                   0     11,568 K
svchost.exe                   5944 Services                   0     12,016 K
dasHost.exe                   6176 Services                   0      7,580 K
svchost.exe                   6488 Services                   0     13,440 K
svchost.exe                   6880 Services                   0     14,412 K
AcerService.exe               6968 Services                   0     28,500 K
conhost.exe                   6988 Services                   0     10,112 K
NgcIso.exe                    7128 Services                   0      4,552 K
svchost.exe                   7368 Services                   0     10,388 K
svchost.exe                   7044 Services                   0     25,428 K
svchost.exe                   7024 Services                   0     57,976 K
svchost.exe                   7240 Services                   0      9,956 K
gamingservicesnet.exe         7292 Services                   0     12,404 K
gamingservices.exe            7260 Services                   0     53,768 K
IntelGraphicsSoftware.Ser     7248 Services                   0     39,724 K
wlanext.exe                   6728 Services                   0      8,524 K
svchost.exe                   8224 Services                   0     35,296 K
AggregatorHost.exe            8472 Services                   0     10,048 K
svchost.exe                   8568 Services                   0     32,320 K
PresentMonService.exe         9096 Services                   0     12,568 K
conhost.exe                   9104 Services                   0      6,196 K
svchost.exe                   8756 Services                   0      5,680 K
AcerSysMonitorService.exe     8528 Services                   0     14,788 K
GameInputRedistService.ex     7584 Console                    1     11,432 K
ipf_helper.exe                8360 Console                    1     11,584 K
sihost.exe                    3952 Console                    1     52,492 K
svchost.exe                   6064 Console                    1     35,072 K
svchost.exe                   8608 Console                    1      7,544 K
svchost.exe                   4140 Console                    1     42,428 K
taskhostw.exe                 2740 Console                    1     22,712 K
svchost.exe                   4156 Services                   0     26,624 K
McUpdaterModule.exe           5024 Console                    1      5,444 K
SSScheduler.exe               9232 Console                    1      6,540 K
explorer.exe                  9736 Console                    1   4,29,760 K
svchost.exe                   9776 Services                   0     24,624 K
svchost.exe                  10144 Services                   0     15,720 K
CrossDeviceResume.exe         9644 Console                    1     66,856 K
svchost.exe                   6404 Services                   0     13,500 K
AICO Out Painting.exe        10216 Console                    1     18,296 K
AICO 2 AC2S.exe               9908 Console                    1      9,300 K
svchost.exe                  10264 Services                   0     49,644 K
FMAudioMonitor.exe           10552 Console                    1     13,440 K
rundll32.exe                 10564 Console                    1     19,276 K
svchost.exe                  10860 Services                   0     20,428 K
svchost.exe                  10988 Services                   0      8,924 K
svchost.exe                  11080 Services                   0     14,172 K
svchost.exe                  11220 Console                    1     44,868 K
svchost.exe                  10076 Services                   0      7,904 K
SearchHost.exe               11356 Console                    1   1,65,312 K
StartMenuExperienceHost.e    11364 Console                    1   1,92,988 K
RtkAudUService64.exe         11512 Console                    1     17,904 K
Widgets.exe                  11652 Console                    1     72,064 K
RuntimeBroker.exe            11804 Console                    1     64,060 K
svchost.exe                  11816 Console                    1     35,312 K
msedgewebview2.exe            9744 Console                    1   1,31,032 K
FMToastNotification.exe      12980 Console                    1     11,832 K
msedgewebview2.exe           12996 Console                    1      9,972 K
msedgewebview2.exe           13504 Console                    1   1,12,160 K
msedgewebview2.exe           13544 Console                    1     44,600 K
msedgewebview2.exe           13656 Console                    1     22,012 K
msedgewebview2.exe           13972 Console                    1   1,15,988 K
NisSrv.exe                    3932 Services                   0     14,280 K
PhoneExperienceHost.exe      14832 Console                    1   1,79,584 K
AcerSysHardwareService.ex    15184 Console                    1     14,872 K
ctfmon.exe                   15352 Console                    1     34,152 K
svchost.exe                   9540 Console                    1     16,040 K
svchost.exe                  14748 Services                   0      9,140 K
svchost.exe                  11036 Console                    1     15,016 K
svchost.exe                   8264 Services                   0      8,220 K
svchost.exe                   5556 Services                   0     16,364 K
ADESv2BW.exe                 15720 Services                   0     10,464 K
TextInputHost.exe            15892 Console                    1   2,02,560 K
SecurityHealthSystray.exe    16244 Console                    1     13,088 K
SecurityHealthService.exe    16188 Services                   0     23,608 K
WmiPrvSE.exe                  8836 Services                   0     13,016 K
WhatsApp.Root.exe             7072 Console                    1   2,43,524 K
SearchIndexer.exe            16548 Services                   0     36,172 K
RuntimeBroker.exe            16780 Console                    1     13,592 K
msedgewebview2.exe           16972 Console                    1   1,62,064 K
msedgewebview2.exe           17032 Console                    1      9,672 K
msedgewebview2.exe           17244 Console                    1   1,85,348 K
msedgewebview2.exe           17252 Console                    1     44,852 K
msedgewebview2.exe           17284 Console                    1     19,216 K
svchost.exe                  17512 Services                   0     17,276 K
ShellExperienceHost.exe      17652 Console                    1   1,24,616 K
AcerGAICameraW.exe           17884 Console                    1     18,812 K
msedgewebview2.exe           18012 Console                    1   3,18,852 K
unsecapp.exe                 18080 Services                   0     10,688 K
AQAUserPS.exe                16184 Console                    1     34,248 K
QuickPanel.exe               15812 Console                    1     82,988 K
QuickPanel.exe                4808 Console                    1     60,336 K
QuickPanelOSD.exe             4820 Console                    1   1,23,952 K
QuickPanel.exe               18268 Console                    1     47,200 K
CefSharp.BrowserSubproces     7592 Console                    1     69,116 K
CefSharp.BrowserSubproces    17976 Console                    1     41,068 K
CefSharp.BrowserSubproces     8244 Console                    1     30,940 K
CefSharp.BrowserSubproces    17136 Console                    1     37,876 K
CefSharp.BrowserSubproces    17764 Console                    1     67,064 K
msedgewebview2.exe           19368 Console                    1     23,052 K
RuntimeBroker.exe            17664 Console                    1     26,436 K
RtkAudUService64.exe          7544 Console                    1     20,256 K
ACCUserPS.exe                19032 Console                    1     11,344 K
OneDrive.exe                 19252 Console                    1   1,49,488 K
WidgetService.exe             3096 Console                    1     28,748 K
msedgewebview2.exe           15060 Console                    1     16,772 K
msedgewebview2.exe            5144 Console                    1      9,652 K
msedgewebview2.exe            8280 Console                    1     11,948 K
msedgewebview2.exe            8516 Console                    1     11,648 K
msedgewebview2.exe            5500 Console                    1          N/A
msedgewebview2.exe            7552 Console                    1      1,124 K
chrome.exe                   17264 Console                    1   2,09,384 K
chrome.exe                   17464 Console                    1      9,496 K
chrome.exe                   11836 Console                    1   3,54,436 K
chrome.exe                   13340 Console                    1     56,584 K
chrome.exe                   15588 Console                    1     21,568 K
msedge.exe                   19676 Console                    1   2,26,700 K
msedge.exe                   19888 Console                    1      9,564 K
msedge.exe                   20168 Console                    1   1,87,820 K
msedge.exe                   20176 Console                    1     56,332 K
msedge.exe                   20384 Console                    1     20,032 K
msedge.exe                   19844 Console                    1   1,76,464 K
RuntimeBroker.exe            21012 Console                    1     21,600 K
svchost.exe                  21076 Services                   0     12,856 K
mscopilot.exe                21944 Console                    1   1,11,548 K
mscopilot.exe                21672 Console                    1      9,512 K
mscopilot.exe                22420 Console                    1     44,084 K
mscopilot.exe                22436 Console                    1     38,424 K
mscopilot.exe                13064 Console                    1     17,148 K
msedge.exe                   22580 Console                    1     21,392 K
svchost.exe                  24588 Services                   0     15,516 K
svchost.exe                  24772 Services                   0     28,488 K
svchost.exe                  24876 Services                   0     15,580 K
svchost.exe                  25004 Console                    1     32,044 K
XboxPcTray.exe               25200 Console                    1     69,516 K
XboxPcAppFT.exe              25240 Console                    1     65,092 K
ApplicationFrameHost.exe     18948 Console                    1     53,044 K
XboxPcApp.exe                24016 Console                    1   1,91,152 K
RuntimeBroker.exe            23424 Console                    1     30,308 K
msedge.exe                   24292 Console                    1   1,14,820 K
msedge.exe                   25428 Console                    1     28,692 K
RuntimeBroker.exe            23568 Console                    1     29,976 K
ONENOTEM.EXE                  8652 Console                    1      3,548 K
msedge.exe                   25304 Console                    1     65,664 K
SystemSettings.exe           15312 Console                    1      1,880 K
svchost.exe                   5988 Services                   0     13,120 K
UserOOBEBroker.exe           20920 Console                    1     11,340 K
msedge.exe                   21044 Console                    1     33,980 K
msedge.exe                    3760 Console                    1     67,512 K
FileCoAuth.exe                4132 Console                    1     32,736 K
WmiPrvSE.exe                  5508 Services                   0     25,088 K
AppActions.exe               15276 Console                    1     46,804 K
mc-webview-cnt.exe           23240 Console                    1      9,092 K
msedgewebview2.exe           19580 Console                    1     34,056 K
msedgewebview2.exe           19896 Console                    1      2,964 K
msedgewebview2.exe           23500 Console                    1     17,392 K
msedgewebview2.exe           23916 Console                    1     17,052 K
msedgewebview2.exe           14036 Console                    1      5,752 K
msedgewebview2.exe            8196 Console                    1      7,504 K
chrome.exe                    3636 Console                    1     77,528 K
chrome.exe                   24544 Console                    1   1,20,704 K
chrome.exe                   12380 Console                    1   1,21,724 K
chrome.exe                   23720 Console                    1     50,496 K
chrome.exe                   11764 Console                    1     23,036 K
LockApp.exe                  10956 Console                    1   1,27,320 K
RuntimeBroker.exe             3056 Console                    1     51,664 K
AICO Parallax Wallpaper.e     7444 Console                    1     18,296 K
AICO AC2S.exe                11052 Console                    1     10,512 K
svchost.exe                  22476 Services                   0      7,852 K
chrome.exe                   16916 Console                    1   2,36,584 K
chrome.exe                   16240 Console                    1   2,07,560 K
svchost.exe                  23624 Services                   0     29,080 K
backgroundTaskHost.exe       22100 Console                    1     61,720 K
RuntimeBroker.exe            13220 Console                    1     31,692 K
cmd.exe                      22304 Console                    1      5,864 K
conhost.exe                  24764 Console                    1     10,208 K
OpenConsole.exe               7396 Console                    1     21,044 K
WindowsTerminal.exe          23680 Console                    1   1,79,028 K
svchost.exe                  12256 Services                   0      9,904 K
chrome.exe                   24456 Console                    1     31,980 K
WmiPrvSE.exe                 24984 Services                   0     13,176 K
TrustedInstaller.exe         19076 Services                   0      9,756 K
TiWorker.exe                 10916 Services                   0     17,916 K
ShellHost.exe                 6960 Console                    1     72,156 K
tasklist.exe                 15648 Console                    1     11,752 K

C:\Users\acer>nslookup
Default Server:  dns64.dns.google
Address:  2001:4860:4860::6464
```
```
C:\Users\acer>whoiami
'whoiami' is not recognized as an internal or external command,
operable program or batch file.
```
C:\Users\acer>whoami
abdul-pc\acer
```

## Result
Thus Execution of Network commands Performed 

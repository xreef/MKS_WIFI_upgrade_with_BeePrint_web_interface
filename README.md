# BeePrint
## MKS WiFi [MISCHIANTI](www.mischianti.org) Web Interface

![](data/launcher-icon-3x.png?raw=true)


##### I am looking for collaborators for the Web interface created in React / Redux, if you are interested write to renzo@mischianti.org. If we manage to form a small group then I will release that part on GitHub as well.

Version 1.4
Thanks to Aleksandr Shell for the russian language translation.
Thanks to [reprapy](https://reprapy.pl/) for the polish language translation.

Version 1.6
Thanks to Ronaldo Risso for Portuguese language

##### Changelog
 - 2023-02-07 BeePrint 1.6.1 MKS WiFi 1.3 Minor fix on Portuguese language and firmware compiled with double MHz (from 80MHz to 160Mhz) for better performance
 - 2023-02-04 BeePrint 1.6 MKS WiFi 1.2 Add Portuguese language (thanks Ronaldo Risso), remaining time and minor fix
 - 2022-02-03 BeePrint 1.5 MKS WiFi 1.2 Better RU translation, fix preload and check the file length
 - 2022-01-08 BeePrint 1.4 MKS WiFi 1.2 Static IP configuration, mDNS, polish translation and minor fix
 - 2022-01-02 BeePrint 1.3 Polish language
 - 2021-12-30 BeePrint 1.2 Add GCode sender widget
 - 2021-12-14 BeePrint 1.1 Add Camera rotation features 
 - 2021-12-03 BeePrint 1.0 Fix the mobile menu on WebView

I bought a FlyingBear Ghost 5 with integrated WiFi module, but I discover that there is no web interface. I don’t know why they can’t add a basic user interface. Then I went to see the web interface the high-end Makerbase cards and realized that it was better they didn’t develop it.

My solution was to modify the firmware to support the Web Socket and develop the Web interface. This feature is compatible with all Makerbase cards that have an MKS WiFi module.

[![Video of the first versione of BeePrint web interface](https://img.youtube.com/vi/VzX84yEbjKM/hqdefault.jpg)](https://www.youtube.com/watch?v=VzX84yEbjKM)


I also decided to explain all the development phases of the project and in this article here I would like to expose the hardware infrastructure of the MKS WiFi card that interfaces with the Makerbase Robin Nano.

 - [MKS WIFI for Makerbase Robin: boards and how to wiring esp12 & NodeMCU](https://www.mischianti.org/2021/11/17/mks-wifi-for-makerbase-robin-boards-and-how-to-wiring-esp12-nodemcu-1/)
 - [MKS WIFI for Makerbase Robin: PCB and how to compile & upload firmware](https://www.mischianti.org/2021/11/21/mks-wifi-for-makerbase-robin-pcb-and-how-to-compile-upload-firmware-2/)
 - [MKS WIFI for Makerbase Robin: communication protocol and Cura plugin](https://www.mischianti.org/2021/11/24/mks-wifi-for-makerbase-robin-communication-protocol-and-cura-plugin-3/)
 - [MKS WIFI for Makerbase Robin: web socket upgrade of the firmware](https://www.mischianti.org/2021/11/28/mks-wifi-for-makerbase-robin-firmware-upgrade-and-new-web-socket-features-4/)
 - [MKS WIFI for Makerbase Robin: BeePrint web interface with Camera on Flying Bear Ghost](https://www.mischianti.org/2021/12/02/mks-wifi-for-makerbase-robin-beeprint-web-interface-with-camera-on-flying-bear-ghost-5/)

I add a Web Socket protocol to manage the communication via Web interface, and I create a responsive and complete Web Interface

![](resources/MKS-WiFi-BeePrint-interface-of-my-FlyingBear-Ghost-5-1024x619.jpg?raw=true)

To prevent speculation over my work I realease all in CC BY NC ND <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/3.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/3.0/88x31.png"></a>
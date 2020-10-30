# DepthAI Open Source Hardware
This repository contains Luxonis open sourced baseboards, and contains Altium design files, documentation, and pictures. This repository is for anyone interested in developing with the DepthAI SoM or anyone interested in understaning more about the embedded hardware that powers DepthAI. 

# Baseboards 

## [BW2098POE](https://github.com/luxonis/depthai-hardware/tree/master/BW2098POE_PoE_Board)
The [BW2098POE repository](https://github.com/luxonis/depthai-hardware/tree/master/BW2098POE_PoE_Board) contains open hardware designed by Luxonis, and meant to be used as a baseboard for the [Luxonis](https://www.luxonis.com/depthai) BW2099 DepthAI SoM. The BW2098POE baseboard offers full 802.3af, Class 3 PoE compliance with 1000BASE-T speeds, along with user-selectable external power from a 5V barrel jack. The Luxonis BW0249 12MP RGB camera module can be connected via the 26-pin FFC interface, which exposes a 4-lane MIPI CSI-2 channel directly into the Myriad X on the BW2099 module for processing. Data can also be streamed to a host via USB 3.1 Gen1 (Type-C). Finally, the BW2098POE board exposes boot selection switches, allowing the end user to boot the BW2099 module from USB or the on-board eMMC or NOR flash.

![](BW2098POE_PoE_Board/Images/BW2098POE_R1M1E1_front.jpg)

## [BW1097](BW1097_DepthAI_Compute_Module)
The [BW1097 repository](/BW1097_DepthAI_Compute_Module) contains open hardware designed by Luxonis, and meant to be used as a baseboard for the [Luxonis](https://www.luxonis.com/depthai) BW1099 DepthAI SoM and the [Raspberry Pi Compute Module 3+](https://www.raspberrypi.org/products/compute-module-3-plus/). Based on the Raspberry PI CMIO board, the BW1097 combines a host and the Luxonis DepthAI SoM to allow for fully integrated solution for real-time spatial AI. 

![](BW1097_DepthAI_Compute_Module/Images/BW1097_R1M1E2_transparent_crop.png)

## [BW1098OBC](BW1098OBC_DepthAI_USB3C)
The [BW1098OBC repository](BW1098OBC_DepthAI_USB3C) contains open hardware designed by Luxonis, and meant to be used as a baseboard for the [Luxonis](https://www.luxonis.com/depthai) BW1099 DepthAI SoM. The BW1098OBC baseboard has three on-board cameras which implement stereo and RGB vision, piped directly into the DepthAI SoM for depth and AI processing. The data is then output to a host via USB 3.1 Gen1 (Type-C). 

![](BW1098OBC_DepthAI_USB3C/Images/BW1098OBC_R1M0E1_front.png)

## [BW1098FFC](BW1098FFC_DepthAI_USB3)
The [BW1098FFC repository](BW1098FFC_DepthAI_USB3) contains open hardware designed by Luxonis, and meant to be used as a baseboard for the [Luxonis](https://www.luxonis.com/depthai) BW1099 DepthAI SoM. The BW1098FFC baseboard has three FFC interfaces which allow for two [BG0250TG](BG0250TG_DepthAI_Mono_Camera) camera modules (stereo pair) and one [BG0249](BG0249_DepthAI_RGB_Camera) RGB camera module. 

![](BW1098FFC_DepthAI_USB3/Images/BW1098FFC_R0M0E0_front.png)

## [BW1094](BW1094_DepthAI_HAT)
The [BW1094 repository](BW1094_DepthAI_HAT) contains open hardware designed by Luxonis, and meant to be used as a baseboard for the [Luxonis](https://www.luxonis.com/depthai) BW1099 DepthAI SoM and as a HAT for the [RPi "B" models](https://www.raspberrypi.org/products/). The BW1094 baseboard has three FFC interfaces which allow for two [BG0250TG](BG0250TG_DepthAI_Mono_Camera) camera modules (stereo pair) and one [BG0249](BG0249_DepthAI_RGB_Camera) RGB camera module. The GPIO interface from the Raspberry Pi Model B variants is passed through the BW1094 with the exception of the 5V pins, GND pins, and [BCM GPIO26 (pin 37)](https://www.raspberrypi.org/documentation/usage/gpio/), which is used as a way for the Raspberry Pi to reset the DepthAI SoM, parallel to the RST button.  

![](BW1094_DepthAI_HAT/Images/BW1094_R0M0E0_front.png)

## [BG0249](BG0249_DepthAI_RGB_Camera)
The [BG0249 repository](BG0249_DepthAI_RGB_Camera) contains open hardware designed by Luxonis. The BW0249 is a carrier board for the Sunny A12N02A IMX378 camera module, and is designed to be compatible with the [BW1094](BW1094_DepthAI_HAT) and [BW1098FFC](BW1098FFC_DepthAI_USB3) baseboards. A 26-pin FFC is used to carry 5V power, 4-lane MIPI, I2C, and other control signals between the BW0249 and the controller baseboards. 

![](BG0249_DepthAI_RGB_Camera/Images/BG0249_R0M0E0_front.png)

## [BG0250TG](BG0250TG_DepthAI_Mono_Camera)
The [BG0250TG repository](BG0250TG_DepthAI_Mono_Camera) contains open hardware designed by Luxonis. The BW0250TG is a carrier board for the Sunny TG161B or AN01V32 OV9282 camera module, and is designed to be compatible with the [BW1094](BW1094_DepthAI_HAT) and [BW1098FFC](BW1098FFC_DepthAI_USB3) baseboards. A 20-pin FFC is used to carry 5V power, 2-lane MIPI, I2C, and other control signals between the BW0250TG and the controller baseboards. A single BG0250TG is typically paired with another to create a stereo camera pair.

![](BG0250TG_DepthAI_Mono_Camera/Images/BG0250TG_R0M0E0_front.png)

## [BK1096](BK1096_OAK-1_Modular)
The [BK1096 repository](/BK1096_OAK-1_Modular) contains open hardware designed by Luxonis, and meant to be used as a baseboard for the [Luxonis](https://www.luxonis.com/depthai) BW1099 DepthAI SoM. The BK1096 baseboard offers a quick and simple way to add USB3 Type-C device power and connectivity, and a single 12MP RGB camera module to the DepthAI SoM. 

![](BK1096_OAK-1_Modular/Images/BK1096_R0M0E0_front.jpg)

asdfas


<!--?xml version="1.0" encoding="UTF-8" standalone="no"?-->
<svg xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:cc="http://creativecommons.org/ns#" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:svg="http://www.w3.org/2000/svg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 210.51138 109.06277" height="109.06277" width="210.51138" xml:space="preserve" id="svg1011" version="1.1"><metadata id="metadata1017"><rdf:rdf><cc:work rdf:about=""><dc:format>image/svg+xml</dc:format><dc:type rdf:resource="http://purl.org/dc/dcmitype/StillImage"></dc:type><dc:title></dc:title></cc:work></rdf:rdf></metadata><defs id="defs1015"><clipPath id="clipPath1029" clipPathUnits="userSpaceOnUse"><path id="path1027" d="M 0,0 H 365760 V 205740 H 0 Z"></path></clipPath></defs><g transform="matrix(1.3333333,0,0,-1.3333333,-3.4343762,536.56561)" id="g1019"><g transform="matrix(1,0,0,-1,0,405)" id="g1021"><g transform="scale(0.0019685)" id="g1023"><g clip-path="url(#clipPath1029)" id="g1025"><g id="g1037"><g id="g1039"><path id="path1041" style="fill:#ffffff;fill-opacity:1;fill-rule:evenodd;stroke:none" d="M 1499,1499 H 81323 V 42671 H 1499 Z"></path></g><path id="path1043" style="fill:none;stroke:#595959;stroke-width:381;stroke-linecap:butt;stroke-linejoin:round;stroke-miterlimit:8;stroke-dasharray:none;stroke-opacity:1" d="M 1499,1499 H 81323 V 42671 H 1499 Z"></path></g><g id="g1045"><g id="g1047"><g id="g1049"><path id="path1051" style="fill:#000000;fill-opacity:0;fill-rule:evenodd;stroke:none" d="M 3882.196,12543.278 H 78942.195"></path></g></g><path id="path1053" style="fill:none;stroke:#595959;stroke-width:1524;stroke-linecap:butt;stroke-linejoin:round;stroke-miterlimit:8;stroke-dasharray:none;stroke-opacity:1" d="M 3882.196,12543.278 H 78942.195"></path></g><g id="g1055"><g id="g1057"><g id="g1059"><path id="path1061" style="fill:#000000;fill-opacity:0;fill-rule:evenodd;stroke:none" d="M 4509.141,3507.0806 H 78309.14 V 11043.08 H 4509.141 Z"></path></g></g></g><g transform="scale(381)" id="g1063"><g transform="translate(11.835016,9.204936)" id="g1065"><g id="g1067"><text id="text1071" style="font-variant:normal;font-weight:bold;font-size:16px;font-family:'Helvetica Neue','Helvetica',Arial,sans-serif;-inkscape-font-specification:HelveticaNeue-Bold;writing-mode:lr-tb;fill:#000000;fill-opacity:1;fill-rule:nonzero;stroke:none" transform="translate(0,15.749763)"><tspan id="tspan1069" y="0" x="0 12.432 22.191999 31.375999 40.848 45.279999 55.647999 65.407997 74.879997 80.991997 90.176003 99.360001 103.792 113.264 117.376 126.56 135.744 145.216 153.808 162.992 171.584">Open Source Licenses </tspan></text></g></g></g><g transform="scale(381)" id="g1073"></g><g id="g1075"><g id="g1077"><g id="g1079"><path id="path1081" style="fill:#000000;fill-opacity:0;fill-rule:evenodd;stroke:none" d="M 4811.468,13579.788 H 40151.47 v 7535.999 H 4811.468 Z"></path></g></g></g><g transform="scale(381)" id="g1083"><g transform="translate(12.628525,35.642487)" id="g1085"><g id="g1087"><text id="text1091" style="font-variant:normal;font-weight:normal;font-size:10.6667px;font-family:'Helvetica Neue','Helvetica',Arial,sans-;-inkscape-font-specification:HelveticaNeue;writing-mode:lr-tb;fill:#000000;fill-opacity:1;fill-rule:nonzero;stroke:none" transform="translate(0,13.629764)"><tspan id="tspan1089" y="0" x="0 7.7013335 13.429334 16.789333 23.104 31.178667 36.90667 40.266666">Hardware</tspan></text></g></g></g><g transform="scale(381)" id="g1093"></g><g id="g1095"><g id="g1097"><g id="g1099"><path id="path1101" style="fill:#000000;fill-opacity:0;fill-rule:evenodd;stroke:none" d="M 4811.468,22147.285 H 40151.47 v 7536 H 4811.468 Z"></path></g></g></g><g transform="scale(381)" id="g1103"><g transform="translate(12.628525,58.129356)" id="g1105"><g id="g1107"><text id="text1111" style="font-variant:normal;font-weight:normal;font-size:10.6667px;font-family:'Helvetica Neue','Helvetica',Arial,sans-;-inkscape-font-specification:HelveticaNeue;writing-mode:lr-tb;fill:#000000;fill-opacity:1;fill-rule:nonzero;stroke:none" transform="translate(0,13.629764)"><tspan id="tspan1109" y="0" x="0 6.9013333 13.024 16.170668 19.52 27.594667 33.322666 36.682667">Software</tspan></text></g></g></g><g transform="scale(381)" id="g1113"></g><g id="g1115"><g id="g1117"><g id="g1119"><path id="path1121" style="fill:#000000;fill-opacity:0;fill-rule:evenodd;stroke:none" d="m 4811.227,30714.783 h 35340 v 7535.997 h -35340 z"></path></g></g></g><g transform="scale(381)" id="g1123"><g transform="translate(12.627893,80.61623)" id="g1125"><g id="g1127"><text id="text1131" style="font-variant:normal;font-weight:normal;font-size:10.6667px;font-family:'Helvetica Neue','Helvetica',Arial,sans-;-inkscape-font-specification:HelveticaNeue;writing-mode:lr-tb;fill:#000000;fill-opacity:1;fill-rule:nonzero;stroke:none" transform="translate(0,13.629764)"><tspan id="tspan1129" y="0" x="0 7.5093336 13.632 19.360001 25.290667 34.389336 40.117336 46.048 49.397335 55.125336 58.474667 60.84267 66.965332">Documentation</tspan></text></g></g></g><g transform="scale(381)" id="g1133"></g><g id="g1135"><g id="g1137"><g id="g1139"><path id="path1141" style="fill:#000000;fill-opacity:0;fill-rule:evenodd;stroke:none" d="M 3882.196,39149.8 H 78942.195"></path></g></g><path id="path1143" style="fill:none;stroke:#595959;stroke-width:1524;stroke-linecap:butt;stroke-linejoin:round;stroke-miterlimit:8;stroke-dasharray:none;stroke-opacity:1" d="M 3882.196,39149.8 H 78942.195"></path></g><g id="g1145"><g id="g1147"><g id="g1149"><path id="path1151" style="fill:#000000;fill-opacity:0;fill-rule:evenodd;stroke:none" d="M 3255.2507,30714.947 H 78315.25"></path></g></g><path id="path1153" style="fill:none;stroke:#595959;stroke-width:381;stroke-linecap:butt;stroke-linejoin:round;stroke-miterlimit:8;stroke-dasharray:none;stroke-opacity:1" d="M 3255.2507,30714.947 H 78315.25"></path></g><g id="g1155"><g id="g1157"><g id="g1159"><path id="path1161" style="fill:#000000;fill-opacity:0;fill-rule:evenodd;stroke:none" d="M 3882.196,21745.566 H 78942.195"></path></g></g><path id="path1163" style="fill:none;stroke:#595959;stroke-width:381;stroke-linecap:butt;stroke-linejoin:round;stroke-miterlimit:8;stroke-dasharray:none;stroke-opacity:1" d="M 3882.196,21745.566 H 78942.195"></path></g><g id="g1165"><g id="g1167"><g id="g1169"><path id="path1171" style="fill:#000000;fill-opacity:0;fill-rule:evenodd;stroke:none" d="M 42970.066,13638.395 H 78310.06 v 7536.001 H 42970.066 Z"></path></g></g></g><g transform="matrix(381,0,0,381,1709.972,0)" id="g1173"><g transform="translate(112.78233,35.796314)" id="g1175"><g id="g1177"><text y="0" x="71.357224" id="text1181" style="font-variant:normal;font-weight:bold;font-size:10.6667px;font-family:'Helvetica Neue','Helvetica',Arial,sans-;-inkscape-font-specification:HelveticaNeue-Bold;text-align:end;writing-mode:lr-tb;text-anchor:end;fill:#000000;fill-opacity:1;fill-rule:nonzero;stroke:none" transform="translate(16.971207,13.629764)"><tspan y="0" x="71.357224" id="tspan1179">MIT</tspan></text></g></g><text id="text1788" y="-45.219803" x="138.91757" style="font-style:normal;font-weight:normal;font-size:40.0001px;line-height:1.25;font-family:sans-serif;fill:#000000;fill-opacity:1;stroke:none;stroke-width:1" xml:space="preserve"><tspan style="stroke-width:1" y="-45.219803" x="138.91757" id="tspan1786"></tspan></text></g><g transform="scale(381)" id="g1183"></g><g id="g1185"><g id="g1187"><g id="g1189"><path id="path1191" style="fill:#000000;fill-opacity:0;fill-rule:evenodd;stroke:none" d="M 42970.066,22205.893 H 78310.06 v 7536 H 42970.066 Z"></path></g></g></g><g transform="scale(381)" id="g1193"><g transform="translate(112.78233,58.283184)" id="g1195"><g id="g1197"><text y="13.629764" x="92.784546" id="text1201" style="font-variant:normal;font-weight:bold;font-size:10.6667px;font-family:'Helvetica Neue','Helvetica',Arial,sans-;-inkscape-font-specification:HelveticaNeue-Bold;text-align:end;writing-mode:lr-tb;text-anchor:end;fill:#000000;fill-opacity:1;fill-rule:nonzero;stroke:none"><tspan style="text-align:end;text-anchor:end" y="13.629764" x="92.784546" id="tspan1199">MIT</tspan></text></g></g></g><g transform="scale(381)" id="g1203"></g><g id="g1205"><g id="g1207"><g id="g1209"><path id="path1211" style="fill:#000000;fill-opacity:0;fill-rule:evenodd;stroke:none" d="M 42969.824,30773.39 H 78309.83 v 7536 H 42969.824 Z"></path></g></g></g><g transform="matrix(381,0,0,381,135.54911,0)" id="g1213"><g transform="translate(112.78169,80.77006)" id="g1215"><g id="g1217"><text y="13.629764" x="92.765083" id="text1221" style="font-variant:normal;font-weight:bold;font-size:10.6667px;font-family:'Helvetica Neue','Helvetica',Arial,sans-;-inkscape-font-specification:HelveticaNeue-Bold;writing-mode:lr-tb;fill:#000000;fill-opacity:1;fill-rule:nonzero;stroke:none"><tspan style="text-align:end;text-anchor:end" y="13.629764" x="92.765083" id="tspan1219">MIT</tspan></text></g></g></g><g transform="scale(381)" id="g1223"></g></g></g></g></g></svg>

asdfasdf



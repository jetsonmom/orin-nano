# orin-nanoHardware Specs


Hardware Layout


대표사진 삭제
사진 설명을 입력하세요.
Part Names

Mark.
Name
Note
1
microSD card slot


2
40-pin Expansion Header


3
Power Indicator LED


4
USB-C port
For data only
5
Gigabit Ethernet Port


6
USB 3.2 Type-A ports (x4)
10Gpbs
7
DisplayPort Output Connector


8
DC Power Jack
5.5mm x 2.5mm
9
MIPI CSI Camera Connectors (x2)
22pin, 0.5mm pitch
10
M.2 Slot (Key-M, Type 2280)
PCIe 3.0 x4
11
M.2 Slot (Key-M, Type 2230)
PCIe 3.0 x2
12
M.2 Slot (Key-E, Type 2230)
(populated)


Port and Connector Details
Note
For the detail, see "Jetson Orin Nano Developer Kit Carrier Board Specification" .

﻿
Storage
Default storage:
microSD card on the Jetson Orin Nano module ( 1 )
Optional storage:
2280-size NVMe SSD card on M.2 Slot (Key-M, Type 2280) ( 10 )
2230-size NVMe SSD card on M.2 Slot (Key-M, Type 2230) ( 11 )
USB drive (on any USB port) ( 4 or 6 )


USB Ports
USB-C port ( 4)
이 USB 3.2 Type-C 커넥터는 호스트, 장치 및 USB 복구 모드를 지원합니다.
주의
이 USB-C 포트는 디스플레이 신호를 출력하는 데 사용할 수 없습니다. USB-C를 통한 HDMI 또는 DisplayPort는 지원되지 않습니다.
Host mode
4개의 Type-A 포트와 마찬가지로 이 포트를 DFP(Downstream-Facing Port)로 사용할 수 있습니다.
           지원되는 USB 장치를 연결하고 Jetson을 호스트로 사용할 수 있습니다.

Device mode
Jetson을 PC에 연결하고(USB-C - Type-A 케이블 또는 USB-C - USB-C 케이블을 통해) Jetson을 USB 장치로 사용할 수 있습니다.
USB Mass Storage Device (to let you mount L4T-README drive)
USB Serial (to provide a serial terminal access)
USB 이더넷(RNDIS) 장치는 PC와 Jetson 사이에 근거리 통신망을 형성합니다(Jetson은 ip주소가 192.168.55.1임니다).
USB Recovery mode
Jetson을 강제 복구 모드로 전환하면 USB 복구 모드에서 작동합니다.

USB 케이블을 통해 Jetson을 PC에 연결하고 PC를 사용하여 Jetson을 flash 할 수 있습니다.
  즉, Jetson을 Force Recovery mode로 설정하면, PC와 Jetson 간에 USB 연결을 통해 Jetson의 
  펌웨어나 소프트웨어를 업데이트하거나 복원하는 등의 작업을 수행할 수 있게  됩니다


USB 3.2 Type-A ports  ( 6 )
이 Type-A 포트를 사용하여 USB 장치를 연결할 수 있습니다. 이들은 호스트 모드 전용입니다.

2개의 이중 스택 유형 A 커넥터가 있으며 각 스택 VBUS는 3A 출력 전류로 제한됩니다.

DisplayPort Output
디스플레이를 개발자 키트에 연결하려면 DisplayPort 출력 포트( 8 )를 사용하십시오. 이것이 개발자 키트에서 디스플레이를 꺼내는 유일한 방법입니다. NVIDIA Jetson Orin Nano 개발자 키트는 USB-C를 통한 HDMI 또는 DisplayPort를 지원하지 않습니다.

HDMI만 허용하는 모니터나 TV에 연결하려면 DisplayPort를 HDMI로 변환하는 어댑터/케이블을 사용할 수 있습니다.
DisplayPort 출력 포트는 패시브 및 액티브 DisplayPort-HDMI(시중에서 DP To HDMI 구입) 어댑터를 모두 지원합니다.

40-pin Expansion Header ( 2 )
Pin assignment :
ORIN NANO
JETSON NANO 2G
 

MIPI CSI Camera Connectors ( 9 )

Jetson Orin Nano 개발자 키트 캐리어 보드에는 CSI 카메라 모듈을 연결하기 위한 22위치 플렉스 커넥터 2개가 포함되어 있습니다.

Raspberry Pi Camera Module v2와 같은 15핀 커넥터로 CSI 카메라 모듈을 연결하려면 15핀에서 22핀으로 변환하는 케이블이 필요합니다.





커넥터는 다음을 지원합니다.

CAM0: CSI 1 x2 lane
CAM1: CSI 1 x2 lane or 1 x4 lane 
이러한 커넥터는 하단 접점, 0.5mm 피치, 22 위치입니다.
부연 설명하자면, 한쪽은 22PIN 다른 한쪽은 15핀으,로 연결됩니다.
 (제슨나노 4GB, 2GB인경우는 15핀으로 된 커넥터가 사용되었다.)



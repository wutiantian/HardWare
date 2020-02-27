<!-- TOC -->

- [Comparison Of Processors 常用处理器的比较](#comparison-of-processors-常用处理器的比较)
- [开发模式](#开发模式)
- [ARM的合作伙伴](#arm的合作伙伴)
- [ARM型号的发展历程](#arm型号的发展历程)
- [三星](#三星)
- [其他半导体厂商](#其他半导体厂商)
- [学生或创客前期开发芯片选择](#学生或创客前期开发芯片选择)
- [公司产品选型](#公司产品选型)

<!-- /TOC -->

# Comparison Of Processors 常用处理器的比较

作者：吴甜甜  时间：2019年6月11日


# 开发模式

- 单片机开发多为裸机，程序规模小，多为单个程序员独立开发。有些复杂产品也会使用高端单片机如STM32之类，并使用RTOS（uCOS、freeRTOS等）。

- 嵌入式开发几乎全部基于嵌入式操作系统，目前使用最多的是linux和Android。

# ARM的合作伙伴

>ARM 合作社区包含 1200 多位伙伴

国际大厂商：
SAMSUNG、TI、ST、
NXP、VLSI、Digital Semiconductor、 Sony、Qualcomm、HP、IBM······
中国授权厂商：
华为海思、全志、瑞芯微、MTK（中国台湾）


![ARM合作商](/images/常用处理器使用比较/ARM合作商.png)

# ARM型号的发展历程




![ARM常用型号列表](/images/常用处理器使用比较/ARM常用型号列表.png)


![ARM发展系列](/images/常用处理器使用比较/ARM发展系列.png)

ARM系列|场景
:---:|:---:
Cortex-A系列<br>（A：Application）|针对日益增长的消费娱乐和无线产品设计，用于具有高计算要求、运行丰富操作系统及提供交互媒体和图形体验的应用领域，如智能手机、平板电脑、汽车娱乐系统、数字电视等。
Cortex-R系列<br>（R：Real-time）|针对需要运行实时操作的系统应用，面向如汽车制动系统、动力传动解决方案、大容量存储控制器等深层嵌入式实时应用。
Cortex-M系列<br>（M：Microcontroller）|该系列面向微控制器领域，主要针对成本和功耗敏感的应用，如智能测量、人机接口设备、汽车和工业控制系统、家用电器、消费性产品和医疗器械等。

# 三星

S3C44B0
S3C2440、S3C2410
S3C6410
S5PV210
Exynos4412 S5P4418

本身使用广泛、有很好的企业应用基础
资料多、积累好，便于学习
开发板和方案商多，软硬件平台好找
体系很典型，适合用来学习

# 其他半导体厂商

Freescale i.MX5系列
TI Omap系列
Qualcomm 骁龙系列
全志科技A10 A20 A31 A33等
行业专用型SoC如华为海思HI3518系列

# 学生或创客前期开发芯片选择

资料多、好找
应用多、有市场需求和底蕴
底层代码无过度封装
难易适中








# 公司产品选型


A架构|型号
---|:---:
Cortex-A5| ATM702x<br>Amlogic M805/S805, T82x<br>Atmel SAMA5D3<br>InfoTM iMAPx820, iMAPx15<br>Qualcomm Snapdragon S4 Play, 200<br>RDA RDA8810PL<br>Telechips TCC892x
Cortex-A7|Allwinner A2x, A3x, A83T, H3, H8<br>NXP i.MX7<br>Broadcom VideoCore BCM2836, BCM23550<br>NXP Semiconductors QorIQ LS10xx Leadcore LC1813, LC1860/C, LC1913, LC1960<br>Marvell Armada PXA1920, 1500 mini plus<br>MediaTek MT65xx<br>Qualcomm Snapdragon 200, 400
Cortex-A8|Allwinner A1x<br>Apple A4<br>Freescale i.MX5<br>Rockchip RK291x<br>Samsung Exynos 3110(S5PC110), S5PV210<br>Texas Instruments OMAP 3<br>Texas Instruments Sitara AM3xxx<br>Texas Instruments DM38x<br>ZiiLABS ZMS-08  
Cortex-A9|Actions ATM702x, ATM703x<br>Altera Cyclone V, Arria V/10<br>Amlogic AML8726, MX, M6x, M801, M802/S802, S812, T86x <br>Apple A5, A5X<br>Broadcom VideoCore BCM21xxx, BCM28xxx<br>Freescale i.MX6<br>HiSilicon K3V2, 910's<br>InfoTM iMAPx912<br>Leadcore LC1810, LC1811<br>Marvell Armada 1500 mini<br>MediaTek MT65xx<br>Nvidia Tegra, 2, 3, 4i<br>Nufront NuSmart 2816M, NS115, NS115M<br>Renesas EMMA EV2, R-Car H1, RZ/A<br>Rockchip RK292x, RK30xx, RK31xx<br>Samsung Exynos 4 421x, 441x<br>ST-Ericsson NovaThor Telechips<br>TCC8803<br>Texas Instruments OMAP 4<br>Texas Instruments Sitara AM4xxx<br>VIA WonderMedia WM88x0, 89x0<br>Xilinx Zynq-7000<br>ZiiLABS ZMS-20, ZMS-40
Cortex-A15|Allwinner A80<br>HiSilicon K3V3<br>MediaTek MT8135/V<br>Nvidia Tegra 4, K1<br>Renesas R-Car H2<br>Samsung Exynos 5 52xx, 54xx<br>Texas Instruments OMAP 5, DRA7xx, AM57xx<br>Texas Instruments Sitara AM5xxx
Cortex-A17|MediaTek MT6595, MT5595<br>Mstar 6A928<br>Rockchip RK3288
ARMv7-A|Apple A6, A6X, S1, S1P, S2, S3<br>Broadcom Brahma-B15<br>Marvell P4J<br>Qualcomm Snapdragon S1, S2, S3, S4 Plus, S4 Pro,<br> 600, 800 (Scorpion, Krait)
processors<br>(64-bit)<br>Cortex-A35|NXP i.MX8X<br>MediaTek MT8516
Cortex-A53|Actions GT7, S900, V700<br>Allwinner A64, H5, H64, R18<br>Altera Stratix 10<br>Amlogic S9 Family, T96x<br>Broadcom BCM2837<br>EZchip TILE-Mx100<br>HiSilicon Kirin 620, 65x, 93x<br>Marvell Armada PXA1928, Mobile PXA1908/PXA1936<br>MediaTek MT673x, MT675x, MT6795, MT873x, MT8752, MT8163<br>NXP ARM S32<br>Qualcomm Snapdragon 41x, 42x, 43x, 61x, 62x<br>Rockchip RK3328, RK3368<br>Samsung Exynos 7 75xx, 78xx<br>Spreadtrum SC9860/GV, SC9836<br>Xilinx ZynqMP<br>NXP Semiconductors QorIQ LS1088<br>NXP i.MX8M
Cortex-A57|AMD Opteron A1100-series<br>NXP Semiconductors QorIQ LS20xx<br>Nvidia Tegra X1<br>Qualcomm Snapdragon 808, 810<br>Samsung Exynos 7 5433, 7420
Cortex-A72|HiSilicon Kirin 95x<br>MediaTek Helio X2x, MT817x<br>Mstar 6A938<br>Qualcomm Snapdragon 65x<br>Rockchip RK3399<br>NXP Semiconductors QorIQ LS2088<br>NXP Semiconductors QorIQ LS1046A<br>NXP i.MX8
Cortex-A73| HiSilicon Kirin 960, Kirin 970<br>MediaTek Helio X30
Cortex-A75|Qualcomm Snapdragon 710, Snapdragon 845
Cortex-A76|HiSilicon Kirin 980<br>Qualcomm Snapdragon 855<br>Samsung Exynos 9820
ARMv8-A|Apple A7, A8, A8X, A9, A9X, A10, A10X, A11, A12<br>Applied Micro X-Gene<br>Cavium ThunderX, ThunderX2<br>Nvidia Tegra K1 (Project Denver)<br>Samsung Mongoose<br>Qualcomm Kryo, Falkor



M架构|型号
---|:---:
Cortex-M0|Cypress PSoC 4000, 4100, 4100M, 4200, 4200DS, 4200L, 4200M<br>Infineon XMC1000<br>Nordic nRF51<br>NXP LPC1100, LPC1200<br>nuvoTon NuMicro<br>Sonix SN32F700<br>STMicroelectronics STM32 F0<br>Toshiba TX00<br>Vorago VA108x0
Cortex-M0+|Cypress PSoC 4000S, 4100S, 4100S+, 4100PS, 4700S, FM0+<br>Holtek HT32F52000<br>Microchip (Atmel) SAM C2, D0, D1, D2, DA, L2, R2, R3<br>NXP LPC800, LPC11E60, LPC11U60<br>NXP (Freescale) Kinetis E, EA, L, M, V1, W0<br>Renesas Synergy S1<br>Silicon Labs (Energy Micro) EFM32 Zero, Happy<br>STMicroelectronics STM32 L0<br>Cortex-M1|Altera FPGAs Cyclone-II, Cyclone-III, Stratix-II, Stratix-III<br>Microsemi (Actel) FPGAs Fusion, IGLOO/e, ProASIC3L, ProASIC3/E<br>Xilinx FPGAs Spartan-3, Virtex-2-3-4
Cortex-M3|Actel SmartFusion, SmartFusion 2<br>Analog Devices ADuCM300<br>Cypress PSoC 5000, 5000LP, FM3<br>Fujitsu FM3<br>Holtek HT32F<br>Microchip (Atmel) SAM 3A, 3N, 3S, 3U, 3X<br>NXP LPC1300, LPC1700, LPC1800<br>ON Semiconductor Q32M210<br>Silicon Labs Precision32<br>Silicon Labs (Energy Micro) EFM32 Tiny, Gecko, Leopard, Giant<br>STMicroelectronics STM32 F1, F2, L1<br>Texas Instruments F28, LM3, TMS470, OMAP 4<br>Toshiba TX03
Cortex-M4|Microchip (Atmel) SAM 4L, 4N, 4S<br>NXP (Freescale) Kinetis K, W2
Cortex-M4F|Cypress 6200, FM4<br>Infineon XMC4000<br>Microchip (Atmel) SAM 4C, 4E, D5, E5, G5<br>Microchip CEC1302<br>Nordic nRF52<br>NXP LPC4000, LPC4300<br>NXP (Freescale) Kinetis K, V3, V4<br>Renesas Synergy S3, S5, S7<br>Silicon Labs (Energy Micro) EFM32 Wonder<br>STMicroelectronics STM32 F3, F4, L4, L4+, WB<br>Texas Instruments LM4F/TM4C, MSP432<br>Toshiba TX04
Cortex-M7F| Microchip (Atmel) SAM E7, S7, V7<br>NXP (Freescale) Kinetis KV5x<br>STMicroelectronics STM32 F7, H7
Cortex-M23|Microchip (Atmel) SAM L10, L11

















<!-- TOC -->

- [arm芯片手册如何读与用](#arm芯片手册如何读与用)
- [芯片手册的架构把握](#芯片手册的架构把握)
- [三星某芯片手册的目录](#三星某芯片手册的目录)
    - [memory controller 存储器控制](#memory-controller-存储器控制)
    - [clock management 时钟管理](#clock-management-时钟管理)
    - [需要什么，就看什么外设的章节](#需要什么就看什么外设的章节)

<!-- /TOC -->

# arm芯片手册如何读与用

作者：吴甜甜

# 芯片手册的架构把握

我们学习单片机，那时是学校的书本，并没有直接给我们厚厚的芯片手册。

但是随着深入学习**嵌入式技术（我指的是可以跑操作系统级别的芯片）**，芯片功能越来越强大，手册也就越来越厚，动辄数千页。

其中，最常用的、标杆手册是**三星**。三星的芯片说明手册规范、详细。

# 三星某芯片手册的目录

模块顺序|章节名称|中文
---|---|---
o|verview|概述
1 |table of contents 
2 |product overview|芯片概述
3 |feature |每一功能的特点
4| block diagram| 芯叶的内部组织结构框图
4.1|core|芯片所选用的arm内核版本
4.2 |periptheral|芯片内部支持的外设控制器
4.3 |bus <AHB .APB.AXI bus>|(芯片内部连接ARM内核与外设控制器的总线）
5| perlptheral controller| 外设控制器的洋细描述章节 
6 |pin assignment|引脚的定义289FBQA (球型封装〉
7| pin number - pin name|引脚的序号,名称
8 |default function|默认功能 (引脚的功能是可以多种选择的，其中有一个是默认的，其他功能是复用到这个管脚的）
9 |signal description |(引脚)佶号描述<br>分类描述（毎一个外设的controller 都负责管理其中一部分自己的管脚多少、方向、功能、作用、复用的种类）
10| special (function) registers|特殊寄存器SFR<br>（每一个controller都有一批自己的寄存器，读写操作就可以来进行软件编程和控制）
10.1| register name|全大写，未来用来宏定义，<br>前面的部分是这个controller的缩写，后边的部分是它的功能。
-|CON  -control| 控制
-|STAT.status |状态
-|DAT -data|
-|MOD-mode| 模式
-|FIFO-filo| 缓冲
-|CFG  -oonfig |配置 
-|CNT counter| 计数
-|TXH transfer holder| 发送缓冲 
-|RXH|
10.2| register addressqu|这个地址，是在写代码的时候，所对应操作寄存器的唯一标识.<br>名宇只是用来助记的，不是内部标识

## memory controller 存储器控制


模块顺序|章节名称|中文
---|---|---
1| memory| 存储布局
-|system memory map|内存映射表（芯片所支持的内存空间的起始他址和结束地址）
-|address space|寻址空间：bank < 一段连续的内存地址，通常会外接到一个存储器的芯片，通常有一个size)<br>这些存储器件可以包括rom和ram (sram (内 部) .norflash.sdram.nandflash)
2| boot rom|启动0地址所在的内存器件，决定启动代码的执行.
-|operation mode (OM)|启动时的操作模式，从哪个器件启动 <br>6410： XOM{4：0] ； 2440: OM[1：0]
3| memory interface|存储器件的接口 (soc和外部存储器件的迕接方式〉 
4| SFR|关于 memory 的 SFR 配置

## clock management 时钟管理


模块顺序|章节名称|中文
---|---|---
0|clock generator block diagram| 时钟发生器的内部结枸 
1|external crystal |供铪cpu的外部晶振的频率 XXPipll  12Mhz外部晶振
2| PLL |锁相环进行倍频 ：有限pll相关的寄存器
3|divider |分频给各个不同的部件；DICN 分频
4| 输出|ARM CLK/FCLK 给 ARM 内核  <br>HCCLK 给 AXI/AHB 高速设备 <br>PCLK  APB 外设  <br>SCLK   给特殊


## 需要什么，就看什么外设的章节


模块顺序|章节名称|重要章节
---|---|---
1| i/O |led beep button pwm seg7 motor switch
2|uart |(getchar putchar)
3| timer |(gettime)
4| interrupt |{timer uart interrupt 
5| DMA |(解放cpu)
6| nandflash |(实现图化）
7| lcd |(驱动液晶) 
8| TS   | （触摸屏0
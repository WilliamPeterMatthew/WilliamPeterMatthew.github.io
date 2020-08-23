---
title: 计算机的组成和程序运行的流程
date: 2020-07-24 14:50:25
---
## 计算机系统的组成
计算机系统分为硬件系统和软件系统。
硬件系统由各个看得见、摸得着的物理实体组件构成，是计算机完成各种操作的物质基础。
软件系统由与操作有关的各种程序以及与之相关的文档和数据的集合组成。其中程序是指用程序设计语言描述的语句指令序列。本书就将带您了解程序设计语言并教您如何编写用程序设计语言描述一序列的语句指令，形成一个程序，来完成一定要求的任务。
没有安装任何软件的计算机俗称“裸机”，是无法正常工作的。硬件系统脱离了软件系统，就会使计算机变成毫无用处的机器；软件系统脱离了硬件系统，就失去了运行的物质基础。因而二者相互依存，不可独立，共同构成了一个完整的计算机系统。

### 计算机硬件系统的基本组成
现代的计算机结构虽然和冯·诺依曼结构有些不太一样，但是仍是基于冯·诺依曼结构的。数学家冯·诺依曼提出了冯·诺依曼结构计算机制造的三个基本原则：
1. 采用二进制逻辑，即计算机内部采用二进制来表示程序以及与之相关的文档和数据。
2. 程序存储执行，即计算机将程序以及与之相关的文档和数据放入同一个存储器（内存储器）中，以供计算机自动高速地从存储器中取出指令加以执行。
3. 计算机硬件由五个基本部分组成：运算器、控制器、存储器、输入设备和输出设备。

计算机硬件的五个基本部分都有相对独立的功能，在控制器的统一有序控制下，各自完成相应的工作。
![1](/book/计算机的组成和程序运行的流程/1.png)

#### 运算器（AU,Arithmetic Unit）
由算术逻辑单元（ALU,Arithmetic Logic Unit）、累加器、状态寄存器、通用寄存器组等组成。算术逻辑单元负责完成加、减、乘、除四则运算和与、或、非、异或等逻辑操作，以及移位、求补等操作。在程序运行时，复杂的运算都将转化为以上的运算，然后在运算器中完成。这些操作会在本书后文提及，此处暂不展开详细介绍。

#### 控制器（Controller）
控制器又叫控制单元（CU,Controller Unit）由程序计数器（PC,Program Counter）、指令寄存器（IR,Instruction Register）、指令译码器、时序产生器和操作控制器（OC,Operation Controller）组成，从内存储器取指令和执行指令，完成协调和指挥整个计算机系统的操作。
控制器与运算器共同组成了中央处理器（CPU,Central Processing Unit）的核心部分，是整个计算机的核心部件，是计算机的“大脑”，控制计算机的运算、处理、输入和输出等工作。

#### 存储器（Memory）
##### 存储器的分类
存储器是用来存储程序和各种数据信息的记忆部件，按存储器的使用类型可分为只读存储器（ROM,Read-Only Memory）和随机存取存储器（RAM,Random Access Memory）。同时存储器可按与CPU联系额密切程度分为内存储器（又叫主存储器，简称内存或主存）和外存储器（又叫辅助存储器，简称外存或辅存）两大类。和CPU直接交换信息的是内存储器。
![2](/book/计算机的组成和程序运行的流程/2.png)

##### 计算机存储单位
计算机存储单位一般以比特（b,bit）和字节（B,Byte）为基本单位计算，其中$1B=8b$。在二者的次方单位中，缩写后缀为小写b即表示为比特的次方单位，缩写后缀为大写B即表示为字节的次方单位。
次方单位前缀存在十进制前缀（SI）和二进制前缀（IEC 60027-2）两种。

<table border="0" cellpadding="0" cellspacing="0" width="864" style="border-collapse:collapse;table-layout:fixed;width:648pt;font-variant-ligatures:normal;font-variant-caps:normal;orphans:2;text-align:start;widows:2;-webkit-text-stroke-width:0px;text-decoration-style:initial;text-decoration-color:initial">
  <colgroup>
    <col width="72" span="12" style="width:54pt">
  </colgroup>
  <tbody>
    <tr height="34" style="height:25.5pt">
      <td colspan="6" height="34" class="xl65" width="432" style="height:25.5pt;width:324pt">比特的次方单位</td>
      <td colspan="6"             class="xl65" width="432" style="              width:324pt">字节的次方单位</td>
    </tr>
    <tr height="21" style="height:15.75pt">
      <td colspan="3" height="21" class="xl75" style="height:15.75pt;border-left:none">十进制前缀（SI）</td>
      <td colspan="3"             class="xl75" style="               border-left:none">二进制前缀（IEC 60027-2）</td>
      <td colspan="3"             class="xl75" style="               border-left:none">十进制前缀（SI）</td>
      <td colspan="3"             class="xl75" style="               border-left:none">二进制前缀（IEC 60027-2）</td>
    </tr>
    <tr height="19" style="height:14.25pt">
      <td height="19" class="xl72" style="height:14.25pt;border-top:none">名字</td>
      <td             class="xl73" style="               border-top:none">缩写</td>
      <td             class="xl74" style="               border-top:none">次方</td>
      <td             class="xl72" style="               border-top:none">名字</td>
      <td             class="xl73" style="               border-top:none">缩写</td>
      <td             class="xl74" style="               border-top:none">次方</td>
      <td             class="xl72" style="               border-top:none">名字</td>
      <td             class="xl73" style="               border-top:none">缩写</td>
      <td             class="xl74" style="               border-top:none">次方</td>
      <td             class="xl72" style="               border-top:none">名字</td>
      <td             class="xl73" style="               border-top:none">缩写</td>
      <td             class="xl74" style="               border-top:none">次方</td>
    </tr>
    <tr height="19" style="height:14.25pt">
      <td height="19" class="xl66" style="height:14.25pt">Kilobit</td>
      <td             class="xl67"                       >Kb</td>
      <td             class="xl68"                       >10³</td>
      <td             class="xl66"                       >Kibibit</td>
      <td             class="xl67"                       >Kib</td>
      <td             class="xl68"                       >2¹⁰</td>
      <td             class="xl66"                       >KiloByte</td>
      <td             class="xl67"                       >KB</td>
      <td             class="xl68"                       >10³</td>
      <td             class="xl66"                       >KibiByte</td>
      <td             class="xl67"                       >KiB</td>
      <td             class="xl68"                       >2¹⁰</td>
    </tr>
    <tr height="19" style="height:14.25pt">
      <td height="19" class="xl66" style="height:14.25pt">Megabit</td>
      <td             class="xl67"                       >Mb</td>
      <td             class="xl68"                       >10⁶</td>
      <td             class="xl66"                       >Mebibit</td>
      <td             class="xl67"                       >Mib</td>
      <td             class="xl68"                       >2²⁰</td>
      <td             class="xl66"                       >MegaByte</td>
      <td             class="xl67"                       >MB</td>
      <td             class="xl68"                       >10⁶</td>
      <td             class="xl66"                       >MebiByte</td>
      <td             class="xl67"                       >MiB</td>
      <td             class="xl68"                       >2²⁰</td>
    </tr>
    <tr height="19" style="height:14.25pt">
      <td height="19" class="xl66" style="height:14.25pt">Gigabit</td>
      <td             class="xl67"                       >Gb</td>
      <td             class="xl68"                       >10⁹</td>
      <td             class="xl66"                       >Gibibit</td>
      <td             class="xl67"                       >Gib</td>
      <td             class="xl68"                       >2³⁰</td>
      <td             class="xl66"                       >GigaByte</td>
      <td             class="xl67"                       >GB</td>
      <td             class="xl68"                       >10⁹</td>
      <td             class="xl66"                       >GibiByte</td>
      <td             class="xl67"                       >GiB</td>
      <td             class="xl68"                       >2³⁰</td>
    </tr>
    <tr height="19" style="height:14.25pt">
      <td height="19" class="xl66" style="height:14.25pt">Terabit</td>
      <td             class="xl67"                       >Tb</td>
      <td             class="xl68"                       >10¹²</td>
      <td             class="xl66"                       >Tebibit</td>
      <td             class="xl67"                       >Tib</td>
      <td             class="xl68"                       >2⁴⁰</td>
      <td             class="xl66"                       >TeraByte</td>
      <td             class="xl67"                       >TB</td>
      <td             class="xl68"                       >10¹²</td>
      <td             class="xl66"                       >TebiByte</td>
      <td             class="xl67"                       >TiB</td>
      <td             class="xl68"                       >2⁴⁰</td>
    </tr>
    <tr height="19" style="height:14.25pt">
      <td height="19" class="xl66" style="height:14.25pt">Petabit</td>
      <td             class="xl67"                       >Pb</td>
      <td             class="xl68"                       >10¹⁵</td>
      <td             class="xl66"                       >Pebibit</td>
      <td             class="xl67"                       >Pib</td>
      <td             class="xl68"                       >2⁵⁰</td>
      <td             class="xl66"                       >PetaByte</td>
      <td             class="xl67"                       >PB</td>
      <td             class="xl68"                       >10¹⁵</td>
      <td             class="xl66"                       >PebiByte</td>
      <td             class="xl67"                       >PiB</td>
      <td             class="xl68"                       >2⁵⁰</td>
    </tr>
    <tr height="19" style="height:14.25pt">
      <td height="19" class="xl66" style="height:14.25pt">Exabit</td>
      <td             class="xl67"                       >Eb</td>
      <td             class="xl68"                       >10¹⁸</td>
      <td             class="xl66"                       >Exbibit</td>
      <td             class="xl67"                       >Eib</td>
      <td             class="xl68"                       >2⁶⁰</td>
      <td             class="xl66"                       >ExaByte</td>
      <td             class="xl67"                       >EB</td>
      <td             class="xl68"                       >10¹⁸</td>
      <td             class="xl66"                       >ExbiByte</td>
      <td             class="xl67"                       >EiB</td>
      <td             class="xl68"                       >2⁶⁰</td>
    </tr>
    <tr height="19" style="height:14.25pt">
      <td height="19" class="xl66" style="height:14.25pt">Zettabit</td>
      <td             class="xl67"                       >Zb</td>
      <td             class="xl68"                       >10²¹</td>
      <td             class="xl66"                       >Zebibit</td>
      <td             class="xl67"                       >Zib</td>
      <td             class="xl68"                       >2⁷⁰</td>
      <td             class="xl66"                       >ZettaByte</td>
      <td             class="xl67"                       >ZB</td>
      <td             class="xl68"                       >10²¹</td>
      <td             class="xl66"                       >ZebiByte</td>
      <td             class="xl67"                       >ZiB</td>
      <td             class="xl68"                       >2⁷⁰</td>
    </tr>
    <tr height="19" style="height:14.25pt">
      <td height="19" class="xl69" style="height:14.25pt">Yottabit</td>
      <td             class="xl70"                       >Yb</td>
      <td             class="xl71"                       >10²⁴</td>
      <td             class="xl69"                       >Yobibit</td>
      <td             class="xl70"                       >Yib</td>
      <td             class="xl71"                       >2⁸⁰</td>
      <td             class="xl69"                       >YottaByte</td>
      <td             class="xl70"                       >YB</td>
      <td             class="xl71"                       >10²⁴</td>
      <td             class="xl69"                       >YobiByte</td>
      <td             class="xl70"                       >YiB</td>
      <td             class="xl71"                       >2⁸⁰</td>
    </tr>
    <!--[if supportMisalignedColumns]-->
      <tr height="0" style="display:none">
        <td width="72" style="width:54pt"></td>
        <td width="72" style="width:54pt"></td>
        <td width="72" style="width:54pt"></td>
        <td width="72" style="width:54pt"></td>
        <td width="72" style="width:54pt"></td>
        <td width="72" style="width:54pt"></td>
        <td width="72" style="width:54pt"></td>
        <td width="72" style="width:54pt"></td>
        <td width="72" style="width:54pt"></td>
        <td width="72" style="width:54pt"></td>
        <td width="72" style="width:54pt"></td>
        <td width="72" style="width:54pt"></td>
      </tr>
    <!--[endif]-->
  </tbody>
</table>

由于混淆已经普遍化，所以所以现在例如MegaByte等十进制前缀单位往往指的是MebiByte等二进制前缀单位。

##### 工作原理
存储器被划分为许多等长的存储单元以便于更好地存放程序以及与之相关的文档和数据。每个存储单元可以存放一个适当单位的信息。全部的存储单元按照一定顺序编号，这个编号就是这个存储单元的地址，简称地址。存储单元与地址是一一对应的。请注意地址和存储单元内的信息是两个东西，不要混淆，这在本书中的部分章节的部分内容中将会体现。
对存储器的操作一般称为访问存储器。访问存储器的方式有两种，一种是选定地址存入数据，称为“写”；另一种是从选定的地址取出数据，称为“读”。当来自地址总线的地址信息传入地址寄存器（MAR,Memory Address Register）后，地址寄存器向地址译码器提供地址信息，然后地址译码器找到对应的存储单元，由读写控制确定访问方式，完成读写操作，数据总线供数据寄存器（MDR,Memory Data Register）传送数据信息使用。
![3](/book/计算机的组成和程序运行的流程/3.png)

#### 输入设备（Input Device）
输入设备是将外部世界信息发送给计算机的设备，是向计算机输入数据和信息的设备，是计算机与用户或其他设备通信的桥梁。
计算机的输入设备按功能可分为字符输入设备（如键盘）、光学阅读设备（如光学标记阅读机、光学字符阅读机）、图形输入设备（如鼠标器、操纵杆、光笔）、图像输入设备（如摄像机、扫描仪、传真机）和模拟输入设备（如语言模数转换识别系统）。

#### 输出设备（Output Device）
输出设备是将处理结果返回给外部世界的设备，是将计算机数据和信息输出的设备。
常见的输出设备有显示器、打印机、绘图仪、影像输出系统、语音输出系统、磁记录设备等。
&emsp;&emsp;
通常我们将输入设备和输出设备统称为I/O（Input/Output）设备，均属于计算机的外部设备。

### 计算机软件系统的基本组成
软件是一系列按照特定顺序组织的电脑数据和指令，是电脑中的非有形部分。
一般来说，计算机软件划分为系统软件和应用软件和介于这两者之间的中间件。

#### 系统软件（System Software）
系统软件主要指用来运行或控制硬件所开发的计算机软件，如操作系统、解释器、编译器、数据库管理系统、公用程序等面向开发者的软件。
系统软件一词常与系统程序（System Program）混用。就狭义而言，系统程序指的是操作系统设计程序，以及与操作系统相关的程序，例如行程排班程序、存储器管理程序、行程通信程序、平行程序程序、驱动程序等等；广义来说，系统程序泛指与计算机系统相关的程序设计程序，例如嵌入式系统、汇编语言程序设计程序、C 语言程序设计程序、Linux 核心程序设计程序等等；而系统软件主要指的是辅佐系统程序能够在电脑上运行或运行特定工作（例如调试程序、行程排班程序）等等的工具程序。

常见的系统软件包含：
- 操作系统（OS,Operating System）：控制与管理计算机硬件与软件资源，并提供用户操作接口，让用户可与计算机交互的系统软件，例如：UNIX、Linux、OS X、Microsoft Windows。
- 编译器（Compiler）：将编程语言撰写的代码，转换成计算机可识读的机器语言，产生可执行文件，例如：GNU C Compiler (GCC)、LLVM，现今许多编译器包含了编译、汇编与链接等多种系统程序功能。
- 解释器（Interpreter）：又叫解译器，能够把高级编程语言逐行直接转译运行，而非将所有内容都转译后才运行。
- 链接器（Linker）：将由编译器或汇编器产生的目标文件和外部程序库链接为一个可执行文件。
- 加载器（Loader）：负责将程序加载到存储器中，并配置存储器与相关参数，使之能够运行，现今许多集成开发环境 (IDE) 集成了编译器与加载器，使的开发人员可以在编译后立即运行测试结果。
- 汇编器（Assembly）：将用汇编语言编写，或是编译器转换过程中产生的汇编语言文件，转换成机器语言文件。
- 调试器（Debugger）：用于调试其它程序，能够让代码在指令组模拟器（ISS）中可以检查运行状况以及选择性地运行（例如设置中断点）。
- 硬件驱动程序（Driver）：它提供了一个软硬件接口，让电脑软件可以与硬件交互的程序。
- 公用程序：管理电脑的许多任务具程序，如:文件管理程序、格式化工具、磁盘管理。

#### 应用软件（Application Software）
又叫应用程序，简称应用（app），是指为针对用户的某种特殊应用目的所撰写的计算机程序，如文本处理器，表格，会计应用，浏览器，媒体播放器，命令行游戏，图像编辑器等。应用软件可以直接完成终端用户的工作。从某种意义上来讲，系统软件是为应用软件服务的，应用软件才是真正直接提高用户工作的。

常见的应用软件类型包括：
- 工业自动化软件（Industrial Automation Software）：工业自动化（Industrial Automation）是指对工业生产线、工艺流程、生产机器进行控制以便减少人工干预的控制系统，而工业自动化软件则是指用于工业控制系统的应用软件，包括数字化控制、可编程逻辑控制器以及其他工业控制系统等。
- 业务软件（Business Software）：业务软件是有助于提高业务生产效率或者度量业务生产效率的应用软件。业务软件又可以细分成多种类型，包括企业软件、企业基础设施软件、信息工作者软件等。需要指出的是，各种类型的软件之间的界限并不是很清晰，有时某种业务软件可能同时属于多种不同的类型。
- 内容访问软件（Content Access Software）：内容访问软件是一种用于访问内容而不是编辑内容的计算机软件。但是，也有些内容访问软件允许用户对内容进行编辑。 这种软件主要是满足对数字化娱乐、出版产品的消费需求。例如，网页浏览器（Web Browsers）、 媒体播放器（Media Players）、数字宠物（Digital Pets）、屏幕保护程序（Screen Saver）、视频游戏（Video Games）等都是典型的内容访问软件。
- 教育软件（Educational Software）：教育软件是一种用于教学或自学的计算机软件。 主要包括儿童学习软件、居家学习软件、教学课件、教学管理软件、娱乐教育软件、教育参考软件、教育软件定制平台、公司培训软件以及特殊教育软件等。
- 仿真软件（Simulation Software）：仿真软件是一种以研究分析、操作培训、娱乐等为目的，模仿真实情景的物理仿真系统或数据仿真系统的计算机软件。仿真软件又可以分为科学仿真、社会仿真、战场仿真、应急响应仿真、飞行驾驶仿真、汽车驾驶仿真、仿真游戏等。
- 多媒体开发软件（Media Development Software）：多媒体开发软件是指用于图形、图像、音频、 视频等多媒体开发的计算机软件。多媒体开发软件又可以分为计算机三维图像软件、计算机动画和图形艺术软件、光栅图形编辑软件、矢量图型编辑软件、视频编辑软件、音频编辑软件、音乐生成器、Web超媒体开发软件等。
- 产品工程软件（Product Engineering Software）：产品工程软件是指辅助相关制造产品的设计、研发、装配的计算机软件。产品工程的主要活动包括成本活动、生产能力、产质量量、产品性能、可靠性、可服务性、用户特征等。产品工程 软件主要包括计算机辅助设计（Computer-Aided Design，CAD）、计算机辅助工程（Computer-Aided Engineering，CAE）、测试工具、游戏创建软件、许可管理程序等。

## 程序运行的流程
### 生成程序的流程
在上文中的系统应用部分，我们已经了解到了编译器、解释器、汇编器和链接器。通常我们将用汇编语言及各种高级语言编写的计算机程序称为源程序（Source Program），把由源程序经过翻译（经过汇编或编译）形成的机器语句指令序列程序称为目标程序（Object Program）。语言处理程序中的汇编器与编译器都具有一个共同的特点就是必须生成目标程序，然后通过执行目标程序得到最终结果，唯一的区别是编译器会先将高级语言源程序翻译为汇编语言再生成目标程序。解释器不产生目标程序，而是借助解释器本身执行源程序。目标程序本身需要与其他代码和库文件通过链接器链接才能生成可执行文件。
![4](/book/计算机的组成和程序运行的流程/4.png)

请注意：除机器语言外，每一种计算机语言都至少具备一种与之相对应的语言处理程序。

### 程序执行的流程
本书中教您编写的程序均可通过命令行解释器（Shell）执行。当用户向命令行解释器输入一行命令后，命令行解释器先判断它是不是一个内置命令，如果不是，命令行解释器会假定用户输入为一个可执行文件的名字，从而去加载并执行该文件。因此，当我们通过编译系统将源文件编译成可执行二进制文件后，在命令行解释器中输入我们得到的可执行二进制文件名，命令行解释器将其从磁盘中加载到主存当中，通过CPU进行解释运行，最终通过终端设备（屏幕）将他显示出来，程序运行结束。

#### CPU的组成
这里我们将进一步对CPU进行深入了解以便于理解程序执行的流程。
CPU是由四大部分所构成的：寄存器、控制器、运算器、时钟。寄存器是CPU内部的内存，程序加载进CPU内部的寄存器中从而被用来解释和运行。时钟是处理操作的最基本的单位，影响着指令的取出和执行时间。控制器和运算器已经在之前的篇目介绍。
CPU中的主要寄存器：
- 累加寄存器（AC,ACC,Accumulator Register）：主要进行加法运算。
- 标志寄存器（PSW,Program Status Word）：记录状态，进行逻辑操作。
- 程序计数寄存器（PC,Program Counter）：是用于存放下一条指令所在单元的地址的地方。
- 基址寄存器（BX,Base Index）：存储当前数据内存开始的位置。
- 变址寄存器（Index）：存储基质寄存器的相对位置，有用来存放相对于DS段之源变址指针的源变址寄存器（SI,Source Index Register）和用来存放相对于ES段之目的变址指针的目的变址寄存器（DI,Destination Index Register）。
- 通用寄存器（GPRs,General Purpose Registers）：支持所有的用法。
- 指令寄存器（IR,Instruction Register）：CPU专用寄存器，用于存储指令。
- 堆栈指针寄存器（SP,Stack Pointer Register）：记录堆栈的起始位置。

#### CPU基本操作
- 加载：把一个字节或一个字从主存复制到寄存器，覆盖掉寄存器中原来的值。
- 存储：把一个字节或一个从寄存器复制到主存，并覆盖主存中原来的值。
- 操作：把两个寄存器的内容复制到ALU，ALU对两个字做算术运算后存回其中的一个寄存器，该寄存器中原来的值会被覆盖。
- 跳转：从cpu执行的指令抽取一个字的内容存入PC，覆盖掉原来的值，从而改变下一条要执行的指令，达到跳转的目的。

### 实例分析
在前面的几个部分中，你已知道计算机的每一个部件的组成以及具体功能，在知道了这些内容后，我会举出两个具体的例子，让你知道程序代码最终形成的机器语言究竟是如何运行的。

#### 取数指令
简单的讲，就是把一个数取出，存到AC（一般加法操作时，AC中的数是被加数）中的具体过程。
1. PC+1，开始指向下一个地址。
2. MAR中存放着下一个地址，根据这个地址指向存储单元中的指令数据。
3. 从存储单元得到数据，存入MDR。
4. 得到指令，格式为指令码+操作码（当前操作就是：取数操作-地址），指令写入IR中。
5. IR询问CU操作种类并得到为取指令操作的回复。
6. 指令中的数据地址存入MAR。
7. 通过MAR得到存储单元中当前地址存储的数据。
8. 得到的数据存入MDR中。
9. MDR中的数据写入AC，完成整个操作。
10. PC+1，开始新一轮的判断。

#### $ax^2+bx+c$程序的运行（已得到可执行文件）
1. 程序由I/O设备送至计算机。
2. PC+1，得到程序首地址。
3. 程序开始启动。
4. 取数指令：PC->MAR->存储单元->MDR->IR。
5. 分析指令：取出IR中的操作码，送入CU得到指令意义。
6. 执行指令：取出IR中的地址码->MAR->存储体->MDR->AC。
7. PC+1，得到新的地址
8. 取数指令：PC->MAR->存储单元->MDR->IR。
9. 分析指令：取出IR中的操作码，送入CU得到指令意义。
10. 执行指令：取出IR中的地址码->MAR->存储体->MDR->X。
11. ……
12. 出现结果
13. 程序执行完毕











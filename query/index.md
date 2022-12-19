# 软件使用须知


<script src="https://kit.fontawesome.com/5519c56e9e.js" crossorigin="anonymous"></script>
<script src="https://assets.salesmartly.com/js/project_3040_3314_1657543658.js"></script>

### Dearun软件简介
<p style="text-indent:2em">Dearun软件包含了当前 DEA 研究领域的主流模型，包括基础效率模型、超效率模型、网络 DEA 模型以及动态 Malmquist 指数分析，可以处理产出包含非期望产出的情形，同时涵盖了在评价时数据为截面类型与面板类型的情形。无需依赖其他环境，操作简单，便于上手。    

**运行系统**：:(fas fa-desktop): Windows 10/ Windows11  64位/32位
### Dearun软件版本介绍
#### Dearun Trial版
网站上直接下载的版本为Dearun Trial版，为功能受限的版本。Trial版包含以下DEA模型：  
- 投入与产出导向的CCR、BCC模型
- 非径向的SBM模型（可包含非期望产出，可选择导向）
- 投入与产出导向的CCR、BCC超效率模型
- Meta-frontier CCR、BCC、SBM模型
- 投入与产出导向的CCR、BCC模型的Malmquist指数（全局参比、相邻参比）
- SBM模型的Malmquist指数（全局参比）
- Meta-frontier CCR、BCC、SBM Malmuqist指数（全局参比）
- 两阶段乘性网络DEA模型     

**注：**
1. Dearun Trial版对数据规模没有限制，理论上可以支持大规模数据集的效率值测算。
2. Trial版软件仅供学习使用，不得用于商业用途。

#### Dearun Standard版
请先下载使用Dearun Trial版本，确保该软件可以在您的电脑上正常使用。Standard版包含以下模型：
- 计算传统Radial模型（CCR、BCC）、SBM模型、Weighted SBM模型、DDF模型、EBM模型、MinDP（至前沿最小距离）、Directional SBM模型、Non-radial DDF模型的效率值
- 可以计算四种主流的交叉效率模型 
- Pessimistic CCR投入导向模型、CCR产出导向模型、SBM模型  
- 可通过ZSG-DEA模型进行资源分配
- 计算传统Radial模型、SBM模型、DDF模型、EBM模型、Directional SBM模型的超效率值
- 可以处理包含非期望产出的情况（除EBM模型外）
- 针对以上模型可以选取不同的规模报酬性，分别是：CRS（constant returns to scale），VRS（variable returns to scale）
- 计算基于**相邻参比**与**全局参比**的CCR、SBM、SBM超效率、DDF、EBM的Malmquist指数模型，并分解为技术进步与效率变化，同时给出计算过程中的效率值  
- 计算经典的ML指数模型与GML指数模型（基于DDF模型）
- 计算基于全局参比的Directional SBM模型、Non-radial DDF模型的Malmquist Luenberger指数与Luenberger指数
- 计算窗口DEA模型，可自行设置窗口期
- 计算Meta-frontier模型、Meta-frontier Malmquist指数模型
- 计算多种基础的两阶段网络DEA模型（包含投入、共享投入、中间产品、产出)

##### Dearun Standard版许可获取方式：
1. 为了更多的研究人员可以快速入手DEA模型，Dearun正在开放下载与许可申请。如您为学术使用用途，将为您提供一定时间的Dearun Standard版许可，许可期内求解次数不限。具体申请方式请返回网站首页，点击`Dearun许可申请`，填写表单进行提交申请，建议准备好数据并整理好格式后申请。审核通过后将发送到邮箱中，收到邮件后请及时激活。
2. 同时也提供长期的软件使用许可，详情请点击页面下方的联系方式进行咨询。

### 常见问题解答
1. 软件支持的数据条目是多少？  
Dearun Trial版与Standard版均没有对数据规模进行限制，指标数也无限制，理论上支持大型数据集。但是需要注意的是，软件计算模型需要时间，如果数据规模较大时，将花费更多的时间进行求解。

2. 软件安装后界面显示不完整怎么办？  
目前软件已经适配了大多数分辨率的情形，但是仍有小部分电脑会出现显示不完整的情况。如果出现这类问题，请参照网站中的兼容性解决方案，并按照流程进行操作。

3. 软件下载后提示有风险怎么办？  
软件是十分安全的，请将其添加到信任列表。

4. 软件对Excel的版本是否有要求？  
理论上是无要求的，但是如果出现导入数据错误的情况，请将数据格式另存为`.xlsx`的后缀，再重新导入尝试。

5. 软件内的数据格式有什么要求？  
在使用软件前，请保证您导入的数据格式符合软件所支持的数据格式。具体数据格式请点击软件中的`帮助`选项，按照要求调整数据。如果数据格式错误，结果肯定是错误的。

6. 软件使用过程中遇到了问题应该如何解决？  
在许可有效期内，如果您在软件操作过程中遇到了问题，可以联系技术支持人员进行解决。

7. 软件计算结果中出现`infeasible`该怎么办？  
说明此时出现了无可行解的情况，即没有找到最优解，如果出现此情况，建议更换模型或者模型假设。

8. 软件提示更新失败怎么办？  
每次使用前请先点击`检查更新`进行版本检查，确保您使用的是`最新版本`，新版本会修复旧版本中的一些BUG，请务必更新。如果提示软件更新失败，请先检查网络，如果网络正常的话，请检查您是否将软件安装在C盘中。如果是由于安装在系统盘而无法进行更新软件的话，请卸载掉当前软件，官网重新下载新版本软件，并将其安装在非系统盘（**如果您事先已经获取了许可文件，请先备份好许可，在安装好新版本文件后，将许可文件重新放入**）。

9. 软件长期使用的有效期分别是多久？  
Dearun Standard版软件提供了半年期与一年期的许可，详情请咨询网站下方的联系方式。

10. 软件是否享有更新服务？  
是的，软件后续的所有版本，均可以进行更新下载。

11. 将许可文件放入后提示错误怎么办？  
如果您将许可文件放入后，软件界面提示错误，请检查许可文件是否放置正确，即放置在软件的安装目录下，并且文件名为`license.lic`的格式。如果提示许可出错，请联系技术支持人员。

12. Dearun软件与SBMrun软件有什么区别？  
SBMrun软件是Dearun软件中有关SBM模型的模块，只能做有关SBM的模型。SBMrun软件是一款专门针对于面板数据的SBM/SBM超效率的相邻/全局参比的Malmquist指数的计算软件，且加入了定制的加速算法，可以很好处理大规模数据的情况。SBMrun Trial版本的软件可支持数据为50行，且也可以计算与SBM模型相关的所有模型。

13. SBMrun软件在计算大规模数据时进度条不动了该怎么办？  
当您的数据规模较大时，例如总数据条目3000行以上，在软件计算过程中，可能会出现进度条不发生变化的情况。如果界面长时间没有变化，请敲击键盘的`Enter`键。

### 用户须知

<p style="text-indent:2em">本软件的版权归Dearun开发者所有，受知识产权法保护。未经作者许可，不得以任何方式复制、分发、修改、翻译、反编译本软件，不得故意删除或者改变软件权利管理电子信息。如有侵权行为，将追究责任。  

The copyright of this software belongs to Dearun developer. All rights are protected by intellectual property law. The software may not be reproduced, distributed, modified, translated or decompiled in any way, nor may the software  information be intentionally deleted or altered without the author's permission. Whoever conducts infringement shall be investigated for responsibility in accordance with the law.

### 结语
<i class="fa-solid fa-award"></i>  大家有什么想法的话，欢迎联系我！谢谢大家的支持~

### Support or Contact
<admin@dearun.top>

# Dearun使用指南


<script src="https://kit.fontawesome.com/5519c56e9e.js" crossorigin="anonymous"></script>
<script src="https://assets.salesmartly.com/js/project_3040_3314_1657543658.js"></script>
## 1 软件简介
&nbsp;&nbsp;&nbsp;&nbsp;<i class="fa-brands fa-fly"></i> 数据包络分析(Data envelopment analysis, DEA) 是一种评价具有多投入和多产出的决策单元(Decision-making unit, DMU)相对有效性的非参数方法，其无需预先给定权重和假设分布，可以直接通过投入与产出数据来确定生产前沿面的结构。作为数学、运筹学与计算机的交叉研究领域，DEA方法在多个领域有着广泛的应用。  

&nbsp;&nbsp;&nbsp;&nbsp;<i class="fa-solid fa-book-bookmark"></i>  大部分刚接触DEA的研究人员，可能都会对这类优化模型有着很深的疑惑，不知从何下手。如果想彻底明白DEA模型的机理，必须熟练掌握并运用运筹学的相关知识，包括如何建立、求解、分析优化模型，这意味着较高的学习成本。目前市面上也有一些软件来处理DEA模型，但是免费的软件只能求解简单的CCR/BCC模型，根本无法满足日常的研究需求。这也是开发本软件的初衷，其中包含了当前DEA研究领域的主流模型，包括基础效率模型、超效率模型、网络DEA模型以及动态Malmquist指数分析，并可以处理存在非期望产出的情形。本文将向您介绍**Dearun**软件的安装、运行流程，便于您更快的上手本软件。  

&nbsp;&nbsp;&nbsp;&nbsp;<i class="fa-solid fa-circle-right"></i>  如果当前网站访问较慢，或者部分图片无法加载，请点击此网站：  [备用链接1](https://dearun.top/dearun/) &nbsp;
[备用链接2](https://dearun.buzz/dearun/)&nbsp;
[备用链接3](https://dearun.club/dearun/)    

{{< style "text-align:right; strong{color:#00b1ff;}" >}}
Dearun软件最新版本： **3.0.1**
{{< /style >}}



## 2 版本信息
### 版本更新信息
> - 每次使用前，请点击`检查更新`按钮来进行版本更新并安装，如有新版本会提示您，新版本会修正旧版本的部分BUG，请**务必进行更新**
> - 1.1.0版本之前，更新需要前往官网下载安装包，并提前备份好获取的`license`文件，安装完毕后，将备份好的`license`文件重新放入安装目录中
> - {{< version 1.1.0 changed >}} 1.1.0版本之后，更新只需要点击`检查更新`按钮，点击确定更新后，将自动下载并安装新版本

{{< version 3.0.1 >}} `更新时间：2022年11月10日` 
**注：本次更新需要重新下载安装包，无法在软件内点击`检查更新`进行更新。**  
<i class="fa-solid fa-check"></i>  “常规效率模型”、“超效率模型”、“网络DEA”选项卡增添了计算面板数据效率值的功能，只需要导入面板数据后，点击“包含时期列”，即可得到面板数据的全局效率值  
<i class="fa-solid fa-check"></i>  加入Pessimistic CCR投入导向、CCR产出导向、SBM模型  
<i class="fa-solid fa-check"></i>  优化了Malmquist指数值的结果显示，输出的格式为面板格式，便于进一步分析，更为直观  
<i class="fa-solid fa-check"></i>  可以设置保存结果后，自动打开结果所在的文件夹，更为方便  
<i class="fa-solid fa-check"></i>  如果在计算前对数据进行了标准化，保存的结果中增添了标准化后的数据表格  
<i class="fa-solid fa-check"></i>  当计算结果出现无可行解时，可以选择是否用1或者0代替结果  
<i class="fa-solid fa-check"></i>  新增了更新许可文件的选项，如果许可提示到期，点击更新即可自动下载最新Trial版许可  
<i class="fa-solid fa-check"></i>  修正了在读取xls格式的文件时，提示导入数据格式错误的问题  
<i class="fa-solid fa-check"></i>  在有网络的情况下，软件启动后会自动检查更新  
<i class="fa-solid fa-check"></i>  Dearun trial版本新增了一个可以直接使用的模型：SBM模型的全局Malmquist指数  
<i class="fa-solid fa-check"></i>  优化了界面UI，提示更为直观，同时修复其他错误  
{{< version 2.1.8-2.1.9 >}} `更新时间：2022年9月27日`  
<i class="fa-solid fa-check"></i>  在无导向SBM模型的基础上新增了投入导向与产出导向的SBM模型  
<i class="fa-solid fa-check"></i>  在无导向SBM超效率模型的基础上新增了投入导向与产出导向的SBM超效率模型    

{{< admonition type=example title="近期版本更新内容 v2.0.0-2.1.7" open=false >}}
{{< version 2.0.7-2.1.7 >}} `更新时间：2022年9月12日`  
<i class="fa-solid fa-check"></i>  提升用户体验，完善了不同模型的提示与注意事项   
<i class="fa-solid fa-check"></i>  修复了部分电脑由于分辨率而导致软件界面显示不全的问题  
<i class="fa-solid fa-check"></i>  优化了Malmquist指数的计算速度         
<i class="fa-solid fa-check"></i>  在Luenberger指数的基础上，新增了Non-radial DDF(NDDF)模型和Directional SBM(SBM-DDF)模型的全局Malmquist-Luenberger指数  
<i class="fa-solid fa-check"></i> 在输入权重或节点类型时不再要求输入英文逗号（如WSBM、NDDF、Network SBM模型）  
<i class="fa-solid fa-check"></i> 新增Dearun Trial，提供软件试用，可计算部分基础模型    
{{< version 2.0.6 >}} `更新时间：2022年8月7日`  
<i class="fa-solid fa-check"></i>  提升用户体验，完善了不同模型的提示与注意事项   
<i class="fa-solid fa-check"></i>  新增了“Min-max标准化”选项，如果数据内有负数、0或量纲差距过大的情况，可以点击该选项进行数据标准化     
<i class="fa-solid fa-check"></i> 新增了Weighted SBM模型、ZSG-DEA模型、两阶段网络SBM模型、两阶段网络SBM超效率模型  
<i class="fa-solid fa-check"></i> 修复之前版本所反馈的BUG  
{{< version 2.0.3-2.0.5 changed>}} `更新时间：2022年7月30日`  
<i class="fa-solid fa-check"></i>  优化界面UI   
{{< version 2.0.1-2.0.2 >}} `更新时间：2022年7月20日`  
<i class="fa-solid fa-check"></i>  优化`帮助`文件打开速度及`检查更新`速度  
<i class="fa-solid fa-check"></i> ML与GML指数中新增`0，y0，-b0弱可处置性`方向  
{{< version 2.0.0 >}} `更新时间：2022年7月18日`  
<i class="fa-solid fa-check"></i> 新增`Non-radial DDF Luenberger指数 -全局参比`与`Directional SBM Luenberger指数 -全局参比`	  
<i class="fa-solid fa-check"></i> 新增`窗口DEA(Windows DEA)`模型，可以自行设定窗口期  
<i class="fa-solid fa-check"></i> 新增`Meta-Frontier`与`Meta-Frontier Malmquist指数`计算方法  
 <i class="fa-solid fa-check"></i> 软件内新增`帮助`按钮，详细介绍了模型选取与数据导入的格式  
{{< /admonition >}}

> 如果您想查更早版本更新信息，请点击下方`以往版本更新内容 v1.0.1-1.1.3`。

{{< admonition type=example title="以往版本更新内容  v1.0.1-1.1.3" open=false >}}
<i class="fa-solid fa-champagne-glasses"></i> **1.1.3 版本更新时间：2022年7月14日**   
<i class="fa-solid fa-check"></i> 优化页面  
<i class="fa-solid fa-check"></i> 为了更直观展示结果，`结果输出表格展示`一栏的数据小数点默认保留5位（而保存在excel内的结果数据仍不受影响，为原始输出结果数据）    
<i class="fa-solid fa-champagne-glasses"></i> **1.1.2 版本更新时间：2022年7月13日**   
<i class="fa-solid fa-check"></i> 新增共享投入两阶段DEA模型及Centralized网络模型    
<i class="fa-solid fa-champagne-glasses"></i> **1.1.1 版本更新时间：2022年6月27日**   
<i class="fa-solid fa-check"></i> 修正当数据量较大时，在模型计算过程中主页面卡顿的问题  
<i class="fa-solid fa-champagne-glasses"></i> **1.1.0 版本更新时间：2022年6月26日**   
<i class="fa-solid fa-check"></i> 优化更新功能，若有新版本，点击检查更新选项，将自动下载更新并安装，无需跳转到官网进行自行更新            
<i class="fa-solid fa-check"></i> 新增Directional SBM模型、Non-radial DDF模型  
<i class="fa-solid fa-check"></i> 新增两种经典的两阶段网络DEA模型（Kao and Hwang, 2008; Chen et al., 2009）     

<i class="fa-solid fa-champagne-glasses"></i> **1.0.8 版本更新时间：2022年6月19日**   
<i class="fa-solid fa-check"></i> 优化界面，提示更加直观        
<i class="fa-solid fa-check"></i> 新增数据初步检查功能（0、空值、非数值）  
<i class="fa-solid fa-check"></i> 优化数据保存功能    
<i class="fa-solid fa-champagne-glasses"></i> **1.0.7 版本更新时间：2022年5月26日**   
<i class="fa-solid fa-check"></i> 修正已知BUG，优化界面显示，不符合所选模型的选项变成了灰色       
<i class="fa-solid fa-check"></i> 新增了四种交叉效率模型        
<i class="fa-solid fa-champagne-glasses"></i> **1.0.6 版本更新时间：2022年5月15日**         
<i class="fa-solid fa-check"></i> 修正了GML指数的计算问题    
<i class="fa-solid fa-champagne-glasses"></i> **1.0.5 版本更新时间：2022年5月15日**  
<i class="fa-solid fa-check"></i> **全新版本，新增若干功能**    
<i class="fa-solid fa-check"></i> DDF输出结果优化，除了会输出beta无效率值外，同时会输出通过转换公式得到的效率值   
<i class="fa-solid fa-check"></i> 新引入基于**相邻参比**与**全局参比**的SBM、SBM超效率、DDF的Malmquist指数模型  
<i class="fa-solid fa-check"></i> 新引入文献的Malmquist-Luenberger（ML）指数模型与Global Malmquist-Luenberger（GML）指数模型    
<i class="fa-solid fa-check"></i> 新增了当计算结果出现无可行解的提示功能  
<i class="fa-solid fa-champagne-glasses"></i> **1.0.4 版本更新时间：2022年5月13日**  
<i class="fa-solid fa-check"></i> 修正包含非期望产出的SBM超效率模型效率展示结果出错的问题，感谢用户@TheChen_的反馈     
<i class="fa-solid fa-champagne-glasses"></i> **1.0.3 版本更新时间：2022年5月4日**  
<i class="fa-solid fa-check"></i> 通过多组数据进行测试，目前已校正好所有模型的结果  
<i class="fa-solid fa-check"></i> 根据相关建议，除SBM模型外，在基础模型CCR与BCC的计算结果中也分别加入了slacks值  
<i class="fa-solid fa-check"></i> 在基础模型CCR与BCC的选取中，分别加入了投入与产出导向  
<i class="fa-solid fa-check"></i> 更改了模型选择界面的菜单栏颜色，更方便您找到输入框  
 
<i class="fa-solid fa-champagne-glasses"></i> **1.0.2 版本更新时间：2022年5月4日**  
<i class="fa-solid fa-check"></i> 修复了软件内点击**检查更新**无反应的问题，感谢评论区@Kai的反馈  

<i class="fa-solid fa-champagne-glasses"></i> **1.0.1 版本更新时间：2022年5月3日**  
<i class="fa-solid fa-check"></i> 修改了已知的BUG，**更快更高更强**  
<i class="fa-solid fa-check"></i> 软件内置了检查更新的功能，若有新版本，将会提示您  
<i class="fa-solid fa-check"></i> 新增了另一种安装方式，无需进行额外配置，一键安装，详见下文（目前已移除之前的安装方式）
{{< /admonition >}}
### 未来版本展望
<i class="fa-solid fa-circle-right"></i> 未来将支持更多的模型，如果您有什么好的提议，欢迎在评论区进行留言 <i class="fa-regular fa-face-smile-wink"></i>    

## 3 下载与安装
> 1. 本软件目前只支持64位Windows系统下载使用，暂不支持mac系统  
> 2. 为方便版本管理，目前已经移除了原始的安装方式 {{< version 1.0.1 changed>}}，如果您之前采用的是第二种安装方式，请删除原来的版本，并按照以下教程进行一键安装
### 下载

 <div style='display: none'>- 点击这里获取Dearun安装文件：<i class="fa-solid fa-file-zipper"></i> [云盘链接](https://share.weiyun.com/DmbYXpTv)，密码：`Dearun`
- 如上述链接无法加载，或者下载较慢，请点击此：[安装包下载](https://app.tmp.link/?tmpui_page=/file&ukey=62b76175bdce4)
> 以上链接请用IE浏览器打开，用手机自带浏览器可能会报错</div>

- 点击这里获取Dearun安装文件：<i class="fa-solid fa-file-zipper"></i> [下载链接 <i class="fa-solid fa-up-right-from-square"></i>](http://1.116.143.157/Dearun_Setup.exe)

{{< admonition type=failure title="下载失败解决方案" open=true >}}
1. 如果点击下载链接没反应，请更换浏览器重试；
2. 如果提示`无法安全下载Dearun_Setup.exe`，请右键点击该提示，在弹出的对话框里选择`仍然保留`，即可开始下载。
{{< /admonition >}}

### 安装
- 请按照以下步骤运行Dearun
1. 点击`Dearun_Setup.exe`文件  
<img src="\images\Dearun_Setup.png" width = "70" height = "70" alt="图片无法加载" align=center /></img>
2. 请跟随安装步骤来即可，建议安装在`D、E盘`等非系统盘  
<img src="\images\安装步骤1.png"  width = "300" height = "200" alt="图片无法加载" align=center /></img>  
<img src="\images\安装步骤2.png" width = "300" height = "200" alt="图片无法加载" align=center /></img>

3. 双击运行桌面上的`Dearun.exe`  
<img src="\images\应用.png" width = "70" height = "70" alt="图片无法加载" align=center /></img>
> **如果您的电脑安装了360软件，由于软件没有数字签名，所以在使用过程中可能会被误判，但是请放心，绝对正常，请将`Dearun.exe`添加为信任文件**  

- **注**  如果打开软件提示license到期，请下载这个文件，并将其复制到软件安装的根目录下：([license下载 <i class="fa-solid fa-up-right-from-square"></i>](http://1.116.143.157/license.lic))，会提示是否覆盖原文件，点击确认即可。**许可的名字不可改变，如果您下载了多个许可文件，导致许可文件后多了数字，如`license(1).lic`，请删除多余的数字，保持`license.lic`的格式。**
<img src="\images\许可安装.png" width = "500" height = "310" alt="图片无法加载" align=center /></img>  
- 顺利的话将会出现如下Dearun图形交互界面：
<img src="\images\展示_3.png" width = "550" height = "390" alt="图片无法加载" align=center /></img>  

<br/> 
{{< admonition type=failure title="软件兼容性问题" open=true >}}
**如果软件界面显示不正常，请参照网站下方的软件兼容性问题解决方案。**    
[软件兼容性问题解决方案 <i class="fa-solid fa-square-pen"></i>](../dearun/#7-软件兼容性问题)  {{< version 2.1.7>}}
{{< /admonition >}}


## 4 Dearun功能介绍

<i class="fa-solid fa-compass"></i> 恭喜您已经成功打开了Dearun，接下来将向您介绍这个软件的功能：
- 计算传统Radial模型（CCR、BCC）、SBM模型、WSBM模型、DDF模型、EBM模型、MinDP（至前沿最小距离）、Directional SBM模型、Non-radial DDF模型的效率值
- 可以计算四种主流的交叉效率模型 
- Pessimistic CCR投入导向模型、CCR产出导向模型、SBM模型  
- 可通过ZSG-DEA模型进行资源分配
- 计算传统Radial模型、SBM模型、DDF模型、EBM模型、Directional SBM模型的超效率值
- 可以处理包含非期望产出的情况（除EBM模型外）
- 针对以上模型可以选取不同的规模报酬性，分别是：CRS（constant returns to scale），VRS（variable returns to scale）
- 选择传统Radial模型，可以判断规模报酬情况（IRS、CRS、DRS）
- 计算基于**相邻参比**与**全局参比**的CCR、SBM、SBM超效率、DDF、EBM的Malmquist指数模型，并分解为技术进步与效率变化，同时给出计算过程中的效率值  
- 计算ML指数模型与GML指数模型
- 计算全局参比的Directional SBM模型、Non-radial DDF模型的Malmquist Luenberger指数与Luenberger指数
- 计算窗口DEA模型，可自行设置窗口期
- 计算Meta-frontier模型
- 计算多种基础的两阶段网络DEA模型（包含投入、共享投入、中间产品、产出)
- 无需额外安装低版本的Excel，兼容性好

<img src="\images\涵盖模型.png" width = "800" height = "300" alt="图片无法加载" align=center /></img>

## 5 软件使用说明
{{< admonition type=tip title="提示" open=True >}}
软件操作指南请点击：[Dearun软件操作指南 <i class="fa-solid fa-up-right-from-square"></i>](../method/)  

**注：此链接的模型介绍与软件操作方法将不再更新！将全部内置在软件界面里 {{< version 2.0.0>}}，请在软件中点击不同模型的`帮助`按钮即可获取更多支持，软件内的帮助会更加详细**
{{< /admonition >}}

## 6 软件许可使用
<i class="fa-solid fa-battery-empty"></i>  直接下载的版本为Dearun Trial版 {{< version 2.1.7>}}，内置`License`，为功能限制的版本，提供了以下普通效率模型的测算:
1. 投入与产出导向的CCR、BCC模型
2. 非径向的SBM模型（可包含非期望产出，可选择导向）
3. 投入与产出导向的CCR、BCC超效率模型
4. Meta-frontier CCR、BCC、SBM模型
5. 投入与产出导向的CCR、BCC模型的Malmquist指数（全局参比、相邻参比）
6. SBM模型的Malmquist指数（全局参比）
7. Meta-frontier CCR、BCC、SBM Malmuqist指数（全局参比）
8. 两阶段乘性网络DEA模型      

<i class="fa-solid fa-compass"></i>   为了更多的研究人员可以快速入手DEA模型，Dearun正在开放下载与许可申请。如您为学术使用用途，将为您提供1天的Dearun Standard版许可，许可期内求解次数不限。具体申请方式请点击[Dearun许可申请 <i class="fa-solid fa-up-right-from-square"></i>](../application/)，填写表单进行提交申请，建议准备好数据并整理好格式后申请。审核通过后将发送到邮箱中，收到邮件后请及时激活。同时也提供长期的软件使用许可，详情请点击页面下方的联系方式进行咨询。

<i class="fa-solid fa-circle-right"></i>  有关软件使用过程中的更多问题请点击 [软件使用须知 <i class="fa-solid fa-up-right-from-square"></i>](../query/)，操作演示数据请点击[示例数据下载 <i class="fa-solid fa-table"></i>](../data/) 获取。
## 7 软件兼容性问题
<img src="\images\兼容性问题1.png" width = "550" height = "600" alt="图片无法加载" align=center /></img>   
**Note**：软件内置的求解器采用的是当今学业与业界评价十分高的开源求解器，本软件基于此求解器进行算法代码的书写，足以解决中小规模的`DEA问题`，且求解速度十分快。由于目前软件的算法实现部分与界面开发功能均由一人完成，难免会出现一些bug <i class="fa-regular fa-face-sad-tear"></i> ，如果您在体验过程中遇到了问题，或者发现计算结果有误，欢迎及时联系我！



## 8 结语
{{< typeit >}}
<i class="fa-solid fa-award"></i>  大家有什么想法的话，欢迎评论区下方留言！ 
{{< /typeit >}}

![高校使用情况词云图](/images/使用高校情况词云图.png "高校使用情况词云图")

## 9 Support or Contact

<i class="fa-brands fa-qq"></i> 2229263318
<a target="_blank" href="http://wpa.qq.com/msgrd?v=3&uin=2229263318&site=qq&menu=yes"><img border="0" src="http://wpa.qq.com/pa?p=2:2229263318:41" alt="点击这里给我发消息" title="点击这里给我发消息"/></a>

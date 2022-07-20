# Dearun使用指南


<script src="https://kit.fontawesome.com/5519c56e9e.js" crossorigin="anonymous"></script>
<script src="https://assets.salesmartly.com/js/project_3040_3314_1657543658.js"></script>
### 软件简介
&nbsp;&nbsp;&nbsp;&nbsp;<i class="fa-brands fa-fly"></i> 数据包络分析(Data envelopment analysis, DEA) 是一种分析决策单元(Decision-making unit, DMU)相对有效性的非参数评价方法，其无需预先给定权重和假设分布，可以直接通过投入与产出数据来确定生产前沿面的结构。作为数学、运筹学与计算机的交叉研究领域，DEA方法在多个领域有着广泛的应用。  
&nbsp;&nbsp;&nbsp;&nbsp;<i class="fa-solid fa-book-bookmark"></i>  大部分刚接触DEA的研究人员，可能都会对这类优化模型有着很深的疑惑，不知从何下手。如果想彻底明白DEA模型的机理，必须熟练掌握并运用运筹学的相关知识，包括如何建立、求解、分析优化模型，这意味着较高的学习成本。目前市面上也有一些软件来处理DEA模型，但是免费的软件只能求解简单的CCR/BCC模型，根本无法满足日常的研究需求。这也是我开发本软件的初衷，其中包含了当前DEA研究领域的主流模型，包括基础效率模型、超效率模型、网络DEA模型以及动态Malmquist指数分析，并可以处理存在非期望产出的情形。本文将向您介绍**Dearun**软件的安装、运行以及使用流程，您可以通过下载文中的`实例数据`进行软件操作，便于您更快的上手本软件。  
&nbsp;&nbsp;&nbsp;&nbsp;<i class="fa-solid fa-circle-right"></i>  如果当前网站访问较慢，或者部分图片无法加载，请点击此网站：[备用链接1](https://dearun.top/dearun/)，[备用链接2](https://dearun.buzz/dearun/)，[备用链接3](https://dearun.club/dearun/)  

{{< admonition type=tip title="License获取与体验" open=True >}}
为了更多的研究人员可以快速入手DEA模型，Dearun正在开放下载与许可申请，Dearun目前为科研工作提供3天的体验期，**请点击此处填写表单申请：**[申请链接](https://www.dearun.top/application)
{{< /admonition >}}


**注：**  
**1.本页面的模型介绍与软件操作方法将不再更新！将全部内置在软件界面里，在软件中点击不同模型的`帮助`按钮即可获取更多支持，软件内的帮助会更加详细！！**  
**2.如果软件下载提示报错，请更换浏览器进行下载；如果安装后提示有风险，请点击`信任本软件`，由于软件没有数字签名，所以会被误杀，软件绝对绿色无毒，请放心使用！**  
### 版本信息
#### 版本更新信息
> - 每次使用前，请点击`检查更新`按钮来进行版本更新并安装，如有新版本会提示您，新版本会修正旧版本的部分BUG，请**务必进行更新**
> - 1.1.0版本之前，更新需要前往官网下载安装包，并提前备份好获取的`license`文件，安装完毕后，将备份好的`license`文件重新放入安装目录中
> - 1.1.0版本之后，更新只需要点击`检查更新`按钮，点击确定更新后，将自动下载并安装新版本

**用户小福利：网络DEA模块目前处于开发初期，所以基础的两阶段网络DEA模型无需license即可使用哦~**  
<i class="fa-solid fa-champagne-glasses"></i> **2.0.0 版本更新时间：2022年7月20日**   
<i class="fa-solid fa-check"></i> ML与GML指数中新增`0，y0，-b0弱可处置性`方向  
<i class="fa-solid fa-champagne-glasses"></i> **2.0.0 版本更新时间：2022年7月18日**   
<i class="fa-solid fa-check"></i> 新增`Non-radial DDF Luenberger指数 -全局参比`与`Directional SBM Luenberger指数 -全局参比`	  
<i class="fa-solid fa-check"></i> 新增`窗口DEA(Windows DEA)`模型，可以自行设定窗口期  
<i class="fa-solid fa-check"></i> 新增`Meta-Frontier`与`Meta-Frontier Malmquist指数`计算方法  
 <i class="fa-solid fa-check"></i> 软件内新增`帮助`按钮，详细介绍了模型选取与数据导入的格式  
<i class="fa-solid fa-champagne-glasses"></i> **1.1.3 版本更新时间：2022年7月14日**   
<i class="fa-solid fa-check"></i> 优化页面  
<i class="fa-solid fa-check"></i> 为了更直观展示结果，`结果输出表格展示`一栏的数据小数点默认保留5位（而保存在excel内的结果数据仍不受影响，为原始输出结果数据）    
<i class="fa-solid fa-champagne-glasses"></i> **1.1.2 版本更新时间：2022年7月13日**   
<i class="fa-solid fa-check"></i> 新增共享投入两阶段DEA模型及Centralized网络模型    
<i class="fa-solid fa-champagne-glasses"></i> **1.1.1 版本更新时间：2022年6月27日**   
<i class="fa-solid fa-check"></i> 修正当数据量较大时，在模型计算过程中主页面卡顿的问题  
> 如果您想查看以往版本更新信息，请点击下方`以往版本更新内容`。

{{< admonition type=example title="以往版本更新内容" open=false >}}
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
#### 未来版本展望
<i class="fa-solid fa-circle-right"></i> 未来将支持更多的模型，如果您有什么好的提议，欢迎在评论区进行留言 <i class="fa-regular fa-face-smile-wink"></i>    

### 下载与安装
> 1. 本软件目前只支持64位Windows系统下载使用，暂不支持mac系统  
> 2. 为方便版本管理，目前已经移除了原始的安装方式，如果您之前采用的是第二种安装方式，请删除原来的版本，并按照以下教程进行一键安装
#### 下载

 <div style='display: none'>- 点击这里获取Dearun安装文件：<i class="fa-solid fa-file-zipper"></i> [云盘链接](https://share.weiyun.com/DmbYXpTv)，密码：`Dearun`
- 如上述链接无法加载，或者下载较慢，请点击此：[安装包下载](https://app.tmp.link/?tmpui_page=/file&ukey=62b76175bdce4)
> 以上链接请用IE浏览器打开，用手机自带浏览器可能会报错</div>

- 点击这里获取Dearun安装文件：<i class="fa-solid fa-file-zipper"></i> [下载链接](http://1.116.143.157/Dearun_Setup.exe)

#### 安装
- 请按照以下步骤运行Dearun
1. 点击`Dearun_Setup.exe`文件  
<img src="\images\Dearun_Setup.png" width = "70" height = "70" alt="图片无法加载" align=center /></img>
2. 请跟随安装步骤来即可，建议安装在`D、E盘`等非系统盘  
<img src="\images\安装步骤1.png" width = "300" height = "200" alt="图片无法加载" align=center /></img>  
<img src="\images\安装步骤2.png" width = "300" height = "200" alt="图片无法加载" align=center /></img>
3. 双击运行桌面上的`Dearun.exe`  
<img src="\images\应用.png" width = "70" height = "70" alt="图片无法加载" align=center /></img>
> **如果您的电脑安装了360软件，由于软件没有数字签名，所以在使用过程中可能会被误判，但是请放心，绝对正常，请将`Dearun.exe`添加为信任文件**  

- **注**  如果打开软件提示license到期，请下载这个文件，并将其复制到软件安装的根目录下：([license下载](http://1.116.143.157/license.lic))，会提示是否覆盖原文件，点击确认即可。

- 顺利的话将会出现如下Dearun图形交互界面：
<img src="\images\展示_1.png" width = "600" height = "400" alt="图片无法加载" align=center /></img>

### Dearun功能介绍
<i class="fa-solid fa-compass"></i> 恭喜您已经成功打开了Dearun，接下来将向您介绍这个软件的功能：
- 计算传统Radial模型（CCR、BCC）、SBM模型、DDF模型、EBM模型、MinDS（至前沿最小距离）、Directional SBM模型、Non-radial DDF模型的效率值
- 计算传统Radial模型、SBM模型、DDF模型、EBM模型、Directional SBM模型的超效率值
- 可以处理包含非期望产出的情况（除EBM模型外）
- 可以计算四种主流的CCR模型交叉效率值  
- 针对以上模型可以选取不同的规模报酬性，分别是：CRS（constant returns to scale），VRS（variable returns to scale）
- 选择传统Radial模型，可以判断规模报酬情况（IRS、CRS、DRS）
- 选择CCR-Malmquist模型，会分解为TFP变化率、效率变化、纯技术效率变动、规模效率变动、技术变化指标  
- 针对SBM模型/SBM超效率模型、EBM模型/EBM超效率模型可以输出相应指标的改进量
- 计算基于**相邻参比**与**全局参比**的SBM、SBM超效率、DDF、EBM的Malmquist指数模型，并分解为技术进步与效率变化，同时给出计算过程中的效率值  
- 计算ML指数模型与GML指数模型
- 计算多种基础的两阶段网络DEA模型（包含投入、中间产品、产出)
- 无需额外安装低版本的Excel，兼容性好

### Dearun使用流程
#### 基础效率模型与超效率模型
- 点击“导入表格”([参考实例数据](/测试数据.xlsx))，请注意表格的导入形式为：

    | DMU名称 | 投入 | 产出 |非期望产出|
    | :------: | :------: | :------: | :------: |
     DMU1 | xxx | xxx | xxx |
     ... | ... | ... |... |
     DMUn | xxx | xxx | xxx| 

{{< admonition warning >}}
**请严格按照投入、产出、非期望产出的顺序进行存放数据**  
{{< /admonition >}}
##### 数据格式检查
- 导入数据后，点击数据格式初步检查中的`截面`选项，进行数据格式检查。
> `数据检查选项`会对您导入的数据进行初步的检查，如是否包含**0值、空值或非数值**(有些同学在整理数据的时候，可能会出现一些excel的错误公式，从而产生非数值的情况，如:#VALUE!)

- 如数据没有上述情况，则有如下输出：`检查结果: 经过初步检查，数据内无空值、0或非数值的情况，请进一步选择模型进行计算。`
<img src="\images\截面数据格式检查.png" width = "500" height = "200" alt="图片无法加载" align=center /></img>
- 如数据存在上述情况，则有如下输出：
<img src="\images\截面数据错误.png" width = "500" height = "200" alt="图片无法加载" align=center /></img>  

{{< admonition >}}
`数据检查选项`只会对数据进行**初步的检查**，没有问题不代表数据格式完全正确，请先保证您的数据是严格按照所需格式进行导入。
{{< /admonition >}}
##### 模型选择及计算
1. 正确导入表格后，会在右边栏出现表格内容
2. 选择需要测算模型，默认**CCR模型 -投入导向**
3. 选择规模报酬性，默认**CRS**
4. 如果选择是DDF模型，请选择合适的方向；若选择的是CCR或SBM模型，“请选择方向”一栏**默认**即可
5. 填写投入变量的个数，如果有2个投入，请填写阿拉伯数字“**2**”，**不要写多余的字**
6. 填写产出变量的个数，同上
7. 填写非期望产出变量的个数，同上，需注意无非期望产出的话，默认即可
8. 点击“开始计算”，右边栏出现计算过程信息
9. 最下面出现计算结果的表格，点击“**结果保存**”，结果将会储存在与你导入数据的**同一个文件夹**内
10. 若测算超效率模型，步骤同上，需注意需要将选项卡切换到`超效率模型`
##### 操作演示
:(fas fa-desktop): 以`SBM模型`为例，数据[同上](/测试数据.xlsx)，包含2个投入，3个期望产出，2个非期望产出：
<iframe src="\静态_.gif"  height="320" width="480" alt="图片无法加载" align=center /></iframe>    

#### 动态效率模型（Malmquist指数）
- 切换选项卡为`Malmquist指数`
- 点击“导入表格”([参考实例数据](/测试数据动态.xlsx))，请注意表格的导入形式为：
    | 时期 | DMU名称 | 投入 | 产出 |非期望产出|
    | :------: | :------: | :------: | :------: | :------: |
      period_1| DMU1 | xxx | xxx | xxx |
      ...| ... | ... | ... |... |
	  period_1| DMUn | xxx | xxx | xxx |
      ...| ... | ... | ... |... |
	  period_m| DMU1 | xxx | xxx | xxx |
      ...| ... | ... | ... |... |
      period_m| DMUn | xxx | xxx | xxx| 

{{< admonition warning >}}
1. **请严格按照 时期、DMU名称、投入、产出、非期望产出 的顺序进行存放数据**
2. **数据纵向排列顺序为：period_1的截面数据、period_2的截面数据……**
{{< /admonition >}}
- 第一列放时期，第二列放DMU名称，第三列之后放指标数据
- 时期按照从小到大的顺序，如2019、2020、2021、2022
- 数据的形式与之前版本有一定的更改，以本格式为准
##### 数据格式检查
- 导入数据后，点击数据格式初步检查中的`面板`选项，进行数据格式检查。
> `数据检查选项`会对您导入的数据进行初步的检查，如是否包含**0值、空值或非数值**(有些同学在整理数据的时候，可能会出现一些excel的错误公式，从而产生非数值的情况，如:#VALUE!)

- 如数据没有上述情况，则有如下输出：`检查结果: 经过初步检查，数据内无空值、0或非数值的情况，请进一步选择模型进行计算。`
<img src="\images\面板数据格式检查.png" width = "500" height = "200" alt="图片无法加载" align=center /></img>
- 如数据存在上述情况，则有如下输出：
<img src="\images\面板数据错误.png" width = "500" height = "200" alt="图片无法加载" align=center /></img>  

{{< admonition >}}
`数据检查选项`只会对数据进行**初步的检查**，没有问题不代表数据格式完全正确，请先保证您的数据是严格按照所需格式进行导入。
{{< /admonition >}}
##### 模型选择及计算
1. 正确导入表格后，会在右边栏出现表格内容
2. 选择需要测算模型，默认**CCR Malmquist 指数模型 -投入导向**
3. 选择规模报酬性，默认**CRS**
4. 填写投入变量的个数，如果有2个投入，请填写阿拉伯数字“**2**”，**不要写多余的字**
5. 填写产出变量的个数，同上
6. 填写非期望产出变量的个数，同上，需注意无非期望产出的话，默认即可
7. 填写测算期数，同上
8. 点击“开始计算”，右边栏出现计算过程信息
9. 最下面出现计算结果的表格，点击“**结果保存**”，结果将会储存在与你导入数据的**同一个文件夹**内
##### 操作演示
:(fas fa-desktop): 以`超效率SBM Malmquist指数-全局参比`为例，数据[同上](/测试数据动态.xlsx)，3个时期，包含2个投入，3个期望产出，2个非期望产出：
<iframe src="\动态_.gif"  height="320" width="480" alt="图片无法加载" align=center /></iframe>   

#### 网络DEA模型  
- 点击“导入表格”([网络dea实例数据](/网络dea实例数据.xlsx))，请注意表格的导入形式为：

    | DMU名称 | 投入 | 中间产品 |产出|
    | :------: | :------: | :------: | :------: |
     DMU1 | xxx | xxx | xxx |
     ... | ... | ... |... |
     DMUn | xxx | xxx | xxx| 

{{< admonition warning >}}
**请严格按照投入、中间产品、产出的顺序进行存放数据**  
{{< /admonition >}}
##### 模型选择及计算
1. 正确导入表格后，会在右边栏出现表格内容
2. 选择需要测算模型，默认**两阶段网络模型(Kao and Hwang, 2008)**
3. 选择规模报酬性，默认**CRS**
4. 投入、中间产品、产出变量个数的填写同上
5. 点击设置，选择在求出整体效率值后，最大化哪一阶段的效率值（0或1），默认第一阶段（详情解释请看下文）
6. 计算出结果后，请点击“**结果保存**”  

:(fas fa-desktop): 以`两阶段网络模型(Kao and Hwang, 2008)`为例，数据[同上](/网络dea实例数据.xlsx)，包含2个投入，2个中间产品，2个产出：
<iframe src="\网络DEA.gif"  height="330" width="480" alt="图片无法加载" align=center /></iframe>   

### 视频演示
<i class="fa-brands fa-bilibili"></i> **数据包络分析（DEA）方法介绍及各类模型（含非期望产出）的计算方法详解及软件实现**
{{< bilibili BV1MS4y1h7gr >}}

>注：上面视频里的面板数据格式为老旧格式，请参照下面这个视频的数据格式   

<i class="fa-brands fa-bilibili"></i>  **超详细的Malmquist、Malmquist-Luenberger指数（相邻、全局参比）处理DEA面板数据的公式与计算方法介绍**
{{< bilibili BV1mS4y1b7ps >}}

<i class="fa-brands fa-bilibili"></i>  **基于Excel深入理解全局Malmquist指数的计算公式与方法**
{{< bilibili BV1Ft4y187jt >}}

### 模型简要介绍（必看）
#### 交叉效率介绍
- 交叉效率的计算均基于CCR模型，`Dearun`分别预设了四种交叉效率模型：
1. 基础交叉效率模型
2. Minimizing total deviation from the ideal point
3. Minimizing the maximum d-efficiency score
4. Minimizing the mean absolute deviation 

{{< admonition type=tip title="交叉效率模型差异" open=True >}}
- 模型1为最基础的交叉效率模型，而模型（2-4）是为了解决交叉效率计算过程中，由于线性规划最优解不唯一而导致的权重向量不唯一的问题，具体论文请参照发表在“Int. J. Production Economics”上的文章“Alternative secondary goals in DEA cross-efficiency evaluation”
- 解决交叉效率结果不唯一的还有经典的 aggresive 及 benevolent策略，也可以解决交叉效率的不唯一问题。但是由于引入的两阶段模型是非线性模型，其次，在引入新的目标后可能仍存在多解，所以本软件不涉及这两种策略
{{< /admonition >}}

- 操作注意事项
1. 在选择模型`交叉效率模型`后，右边的`设置`按钮变为可选择状态，点开后，会出现如下界面：
 <img src="\images\交叉效率结果.png" width = "620" height = "200" alt="图片无法加载" align=center /></img>  
2. 选择你所需要的交叉效率模型，点击一下对应的选项即可。其中MTDFIP、MMDS、MMAD均是在原有基础上引入第二阶段的目标函数，结果可能会相同，具体请参照上述提到的论文
3. 上述交叉效率模型无法处理非期望指标，因为均是基于CCR模型提出，所以如果有非期望产出，请自行转为投入指标
#### SBM模型介绍
##### 普通SBM模型结果解读  
- 对于普通SBM模型来说，采用的是Tone2001年及2007年的文章进行建模计算（2007年定义的包含非期望产出的SBM形式）。   
- 在计算结果里slack都是正的，投入slacks代表的是投入需要减少的量、产出slacks代表的是产出需要增加的量，非期望产出slacks代表的是非期望产出需要减少的量    

**例**：对于DMU1，投入slack=1，产出slack=1，非期望产出slack=1，分别代表投入需要缩减1，产出需要扩增1，非期望产出需要缩减1，这样DMU1才是有效的

##### 超效率SBM模型结果解读   
- 对于超效率SBM模型来说，只需要对普通SBM模型里等于1的DMU代入超效率模型中进行计算，采用的是Tone2002的文章进行建模计算。  
- 在计算结果里，**对于小于1的，用的仍是SBM模型，slack的含义同上**   
- 对于大于1的，采用超效率SBM模型，为了与效率小于1的slack示以区分，**slack全部标记负号，代表着超出前沿的量**   

**例**：对于DMU1，如果效率大于1，且投入slack=-1，产出slack=-1，非期望产出slack=-1，代表投入扩增1，产出缩减1，非期望产出扩增1（均为反向变化），DMU1经过这样的变化后，**仍然是有效的**，从而体现了一种“超”效率的思想

#### Directional SBM模型与Non-radial DDF模型
- Directional SBM模型与Non-radial DDF模型通过设定合适的权重或方向，两者可以相互转换，本质上是类似的模型，这里给出经典的模型定义式。
1. Directional SBM模型：Fukuyama H, Weber W L. A directional slacks-based measure of technical inefficiency[J]. Socio-Economic Planning Sciences, 2010, 43(4): 274-287.  
<img src="\images\方向SBM.png" width = "600" height = "200" alt="图片无法加载" align=center /></img>
> 在Directional SBM模型中，采用的是论文中比较常见的方向向量，默认为`x0,y0,b0`。
2. Non-radial DDF模型：Barros C P, Managi S, Matousek R. The technical efficiency of the Japanese banks: Non-radial directional performance measurement with undesirable output[J]. Omega, 2012, 40: 1-8.  
<img src="\images\NDDF.png" width = "500" height = "200" alt="图片无法加载" align=center /></img>  

{{< admonition >}}
1. 在Non-radial DDF模型，可自行选择方向向量，默认为`-x0,y0,-b0弱可处置性`，您也可以根据选项卡设置`-x0,y0,-b0强可处置性`。（**用的比较多的是第一种弱可处置性及第二种强可处置性形式，建议选择这两种方式**）
2. 权重向量需要用户点击`设置`选项自行指定。若指标数有n个，对应需要填写n个权重值，且权重值之前请用英文逗号`,`进行隔开。如有5个指标，设定相等权重值，则弹出窗口请填写`1/5,1/5,1/5,1/5,1/5`（如下）  
<img src="\images\权重设定.png" width = "400" height = "300" alt="图片无法加载" display="table-cell" text-align="center"/></img>
{{< /admonition >}}


#### EBM模型介绍
##### 模型背景
- EBM（epsilon-based measure）模型是由Tone和Tsutsui于2010年提出的模型，融合了径向与SBM模型，将指标的改进分为了径向改进及松弛改进两部分，不同指标的处理方式不同。具体思想是通过原始数据先计算有效的投影值矩阵，并引入“affinity index”，用来定义投入/产出数据之间的“affinity matrix”，从而推导出EBM模型的两个参数`ε`及`w`，将原始数据代入EBM模型中进行计算，从而得到最优效率值。

{{< admonition type=tip title="Tips" open=True >}}
- 原文为Tone在2010年发表在EJOR上的文章“An epsilon-based measure of efficiency in DEA – A third pole of technical efficiency”
- 模型的引入背景及优点为：In DEA, we have two measures of technical efficiency with different characteristics: radial and non-radial. In this paper we compile them into a composite model called ‘‘epsilon-based measure (EBM).” For this purpose we introduce two parameters which connect radial and non-radial models. These two parameters are obtained from the newly defined affinity index between inputs or outputs along with principal
component analysis on the affinity matrix. Thus, EBM takes into account diversity of input/output data and their relative importance for measuring technical efficiency.（摘自原文）
{{< /admonition >}}
##### 计算过程
1. 先将所有数据通过ADD模型或SBM模型投影到有效前沿上：   
<img src="\images\投影值计算.png" width = "400" height = "500" alt="图片无法加载" align=center /></img>
2. 得到投影矩阵：  
<img src="\images\EBM步骤1.png" width = "350" height = "130" alt="图片无法加载" align=center /></img>
3. 计算所需参数：   
<img src="\images\EBM步骤2.png" width = "400" height = "200" alt="图片无法加载" align=center /></img>
4. 代入EBM模型：  
<img src="\images\EBM步骤3.png" width = "400" height = "150" alt="图片无法加载" align=center /></img>
> - 步骤3仅给出了对于产出系数的计算方式，投入也是一样的处理方式
> - 步骤3中省略了affinity matrix的部分计算过程，具体步骤请参照原文
> - 除此之外，在步骤4的模型中，加入了对θ和η的限制，分别要求θ小于等于1，η大于等于1，防止出现投入的径向改进量θ大于1的情况，产出同理
> - Dearun在投影值的计算中，采用的是SBM模型
> - EBM模型暂时不能处理非期望产出，如有非期望产出，请将其转为投入
##### 结果分析
- 选项卡选择`EBM`模型，设定好投入与产出，点击开始计算，`求解信息展示`栏会出现以下结果：
<img src="\images\EBM结果分析.png" width = "500" height = "510" alt="图片无法加载" align=center /></img>
- 模型中的epsilon参数为: `[0.48795723531095225, 0.47644560744724607]`分别代表投入和产出的`ε`值
- 指标权重为: `{'输入1': 0.5000000000000001, '输入2': 0.5, '输出1': 0.3169771854782232, '输出2': 0.3463965934614732, '输出3': 0.33662622106030354}` 分别代表投入、产出不同指标的权重值，并均以进行归一化处理
- `结果输出展示`中会给出投入和产出的径向效率值及松弛改进，投入的径向改进为`sita`，产出的径向改进为`fai`
#### DDF模型的方向介绍
- DDF的方向及可处置性预设了以下四种：   
  <img src="\images\DDF方向.png" width = "300" height = "300" alt="图片无法加载" align=center /></img>  

这四种方向及可处置性分别对应的非期望产出的处理方式为： 
- $(-x_0,y_0,-b_0)$弱可处置性$=$： 
  $\sum_{j=1}^{n} \lambda_{j} b_{t j} =(1-\beta) b_{t0}$
- $(-x_0,y_0,-b_0)$强可处置性$\leq$： 
  $\sum_{j=1}^{n} \lambda_{j} b_{t j} \leq (1-\beta) b_{t0}$
- $(-x_0,y_0,-b_0)$强可处置性$\geq$：
  $\sum_{j=1}^{n} \lambda_{j} b_{t j} \geq (1-\beta) b_{t0}$
- $(-x_0,y_0,b_0)$强可处置性$\leq$：
  $\sum_{j=1}^{n} \lambda_{j} b_{t j} \leq (1+\beta) b_{t0}$  

{{< admonition type=info title="如何确定方向和可处置性？" open=True >}}
- 以上四种方向均有论文采用，具体选取什么方向请自行决定，**用的比较多的是第一种弱可处置性及第二种强可处置性形式，建议选择这两种方式**
    
注：以上四种方向中的投入及期望产出均为强可处置性
{{< /admonition >}}

除对非期望产出的处理方式不同外，目标函数与其他约束条件均相同。  
**目标函数均为：**
$\max \beta$  
**投入和期望产出的约束均为:**  
$\sum_{j=1}^{n} \lambda_{j} x_{i j} \leq(1-\beta) x_{i0}$  
$\sum_{j=1}^{n} \lambda_{j} y_{r j} \geq(1+\beta) y_{r0}$  

{{< admonition type=tip title="DDF输出结果解析" open=True >}}
DDF模型的输出结果分为两列，第一列为$\beta$值，指的是DDF模型中算出的$\beta$无效率值，0为有效，数值越大越无效；我们习惯的效率值都是在0到1之间的，所以这里通过计算公式：$ efficiency= (1-\beta)/(1+\beta)$将$\beta$值转为效率值，1为有效，数值越大越有效，并将结果展现在第二列中。
{{< /admonition >}}
#### Malmquist模型介绍
- `Dearun`可以求解以下几种Malmquist指数模型：  
  <img src="\images\M指数_.png" width = "300" height = "200" alt="图片无法加载" align=center /></img>  
##### Malmquist模型结果分析
- 在表格结果中，`e-t-t+1_0`代表第t+1期的DMU相比于第t期参考集的效率值$D^{t}\left(x^{t+1}, y^{t+1}, b^{t+1}\right)$，其他同理；在全局参比的结果中，`e-g-t+1_0`代表第t+1期的DMU相比于全局参考集的效率值$D^{G}\left(x^{t+1}, y^{t+1}, b^{t+1}\right)$，其他同理。
- 每一个时期的结果分为7列，前四列（`e-xx-xx_i`的形式）均为指数的计算过程，无需关注；只需考察每个时期的后三列，`effch`表示效率变化，	`techch`表示技术进步，`tfpch`表示TFP指数的变化率。
- `effch、techch、tfpch`后面的数字`i`代表第i期的结果，如果有四年：2019，2020，2021，2022年，`i=0`代表2019-2020年的指数值；`i=1`代表2020-2021年的指数值，以此类推。
##### M指数、ML指数与GML指数计算方式
- ①Malmquist指数计算方式如下：  

<img src="\images\M.png" width = "500" height = "180" alt="图片无法加载" align=center /></img>
- ②全局Malmquist指数计算方式如下：
<img src="\images\GM.png" width = "500" height = "180" alt="图片无法加载" align=center /></img>
- ③Malmquist-Luenberger计算方式如下：
$$ 
<img src="\images\ML.png" width = "600" height = "130" alt="图片无法加载" align=center /></img>
$$  
- ④Global Malmquist-Luenberger计算方式如下：  
<img src="\images\GML.png" width = "500" height = "180" alt="图片无法加载" align=center /></img>  
> 注：以上所有公式均来自原论文

{{< admonition type=tip title="Malmquist指数计算其他注意事项" open=True >}}
- 因为用`相邻参比`算跨期效率时，相当于计算超效率值，所以会出现无可行解的情况，并且`VRS`假设下更容易出现无可行解，读者可以先用`相邻参比`来计算Malmquist指数值；如果出现无可行解的情况，可以选择`全局参比`来计算指数。
- 基于SBM模型与SBM超效率模型的`相邻参比`Malmquist指数模型一般不会出现无可行解。
- `EBM Malmquist指数 -相邻参比`、`超效率EBM Malmquist指数 -相邻参比`除了会给出指数分解值外，在`求解信息展示`栏还会给出每一期的参数`ε`及`w`，具体定义与上一节EBM模型中的定义相同，用户可以根据需求进行保存参数
- `EBM Malmquist指数 -全局参比`、`超效率EBM Malmquist指数 -全局参比`除了每一期的参数`ε`及`w`外，还会给出全局的参数`ε`及`w`，用`all`进行表示
- `DDF Malmquist指数 -相邻参比`与`DDF Malmquist指数 -全局参比`中本期及跨期效率值的计算方式为$ efficiency= (1-\beta)/(1+\beta)$，之后采用公式①或②进行计算。
- Malmquist-Luenberger（ML）指数模型同样是基于DDF模型的，与`DDF Malmquist指数 -相邻参比`的区别是：指数的计算方式不同，ML指数模型的计算方式参考文献为：**Chung et al.（1997） 的 “Productivity and undesirable outputs: A directional distance function approach”**，指数计算方式为公式③。
- Global Malmquist-Luenberger（GML）指数模型同样是基于DDF模型的，与`DDF Malmquist指数 全局参比`的区别是：指数的计算方式不同，GML指数模型的计算方式参考文献为：**Oh(2010) 的“A global Malmquist-Luenberger productivity index”**，指数计算方式为公式④。   
{{< /admonition  >}}

#### 网络DEA模型介绍
##### 基础两阶段模型
- 目前软件加入两种经典的两阶段网络DEA模型，生产过程为：
<img src="\images\两阶段生产过程.png" width = "500" height = "180" alt="图片无法加载" align=center /></img>
> 这两种模型，第一阶段的产出需全部作为第二阶段的投入  

{{< admonition type=quote title="参考文献" open=True >}}
- 两个模型参考的文献分别为：  
1. Kao C, Hwang S N. Efficiency decomposition in two-stage data envelopment analysis: An application to non-life insurance companies in Taiwan[J]. European Journal of Operational Research, 2008, 185(1): 418-429.  
2. Yao C, Cook W D, Ning L, et al. Additive efficiency decomposition in two-stage DEA[J]. European Journal of Operational Research, 2009, 196(3): 1170-1176.  
{{< /admonition >}}
- 两个模型的区别主要是：整体效率和两个子阶段效率之间的关系分别是multiplicative和additive的，且Kao and Hwang(2008)的模型只支持CRS约束下的计算，而Yao et al.(2009)在CRS和VRS假设下均可以计算，具体模型形式请大家参考原文（如下给出了Yao et al., 2009的模型形式）。  
<img src="\images\网络DEA模型形式.png" width = "300" height = "550" alt="图片无法加载" align=center /></img>
- 前文在网络DEA操作介绍中给的实例数据为两篇论文中原文所采用的数据，由于原文中数据的数量级过大，防止计算中出现数值问题，所以对所有指标下的数据同除以了10000，结果仍然与原文是相同的。   
<i class="fa-brands fa-bilibili"></i>  **[第一弹]网络DEA模型发展及经典模型的解读与计算（共享投入、两阶段网络DEA）**
{{< bilibili BV1k34y1n7pu >}}  
##### 进阶两阶段模型
- 共享投入两阶段模型  
<img src="\images\共享投入两阶段生产过程.png" width = "500" height = "180" alt="图片无法加载" align=center /></img>  
- Centralized两阶段模型  
<img src="\images\Centralized两阶段生产过程.png" width = "500" height = "180" alt="图片无法加载" align=center /></img>  
{{< admonition type=quote title="参考文献" open=True >}}
- 两个模型参考的文献分别为：  
1. Yao C, Du J, Sherman H D, et al. DEA model with shared resources and efficiency decomposition[J]. European Journal of Operational Research, 2010, 207(1): 339-349.  
**文章数据：**[链接](/共享测试数据.xlsx)
2. Li Y, Chen Y, Liang L, et al. DEA models for extended two-stage network structures[J]. Omega, 2012, 40( 5):611-618.  
**文章数据：**[链接](/CentralizedmodelData.xlsx)
{{< /admonition >}}  
<i class="fa-brands fa-bilibili"></i>  **[第二弹]网络DEA模型发展及经典模型的解读与计算（共享投入、两阶段网络DEA）**
{{< bilibili BV1zT411J7R3 >}}
- 共享投入两阶段模型需要设置每个共享投入在第一阶段的比例范围，详情请参照教程视频。



- **后期将支持更多的网络DEA模型，尽请期待**。 




### Dearun注意事项
> 请逐条仔细阅读下列注意事项
- 如果数据表格导入有误，将会出现`Error:数据读取有误，请检查数据`的字样，那么请您重新检查数据格式
- 一定要注意数据 <i class="fa-solid fa-file-circle-check"></i> 的正确格式，在静态模型中，第一列放DMU名称，第二列开始按照投入、产出、非期望产出的顺序放置数据，在动态模型中，第一列放时期，第二列开始按照DMU名称、投入、产出、非期望产出的顺序放置数据，确保数据准确无误，否则计算结果将出错
- 请注意指标里**不能出现负数据、0数据**，如果出现上列数据，请自行进行处理为正数据，本软件不内置处理方法
- 数据正常导入后，点击`开始计算`后若出现`出错，请检查步骤是否正确`，那么请您检查是否按照上述步骤进行操作
- 在导入数据后，您可以多次测算模型，并通过最下方查看计算的结果
- **在使用CCR模型处理非期望产出指标时，会默认将非期望产出归于投入指标来进行计算**（在基础CCR、超效率CCR，Malmquist CCR均采用这样的处理方式）
- CCR的CRS与VRS假设下均会给出技术效率、纯技术效率、规模效率及规模报酬情况，但是需要注意松弛改进量是不同的，与您选择的假设有关
- 请注意**使用涉及到DDF的相关模型时必须选取方向**，如果不选取方向将无法进行求解 <i class="fa-regular fa-face-sad-tear"></i> 
- SBM与EBM模型软件内置的均为非导向，没有投入/产出导向的SBM、EBM，因为使用情况特别少
- 如在使用除DDF的模型外，方向选择一栏将变灰
- 只有选择交叉效率模型，`设置`选项才可以进行选取，默认普通交叉效率
- 在使用`Malmquist模型`时务必正确填写`期数`，如果不填写期数将无法进行求解 <i class="fa-regular fa-face-sad-tear"></i> 
- 使用超效率模型时或使用VRS假设时，会由于模型不可行的问题导致无法产生最优解，会在表格里进行标注`infeasible`，并会在信息框中提示您。如果出现了无可行解，建议您更换规模报酬假设、更换方向或更换模型
- 数据量纲不能差距太大，如出现量纲差距很大，请先调整量纲，否则结果可能会出错
- 由于精度问题，结果会出现0.9999999999或者1.000000000001这类型的数据，这些都视为效率等于1
- 如果您需要保存数据，请务必按下“**结果保存**”键，否则不会对结果进行保存
- 用到的所有模型均是基于原始论文继续复现
- 软件提供了检查更新的功能，运行后可以点击右下角的`检查更新`，如果有新版本，将会提醒您去官网安装新版本
- 如果出现点击“**结果保存**”键没反应的情况，可能是您之前保存过同样的模型结果，且excel文件保持打开的状态，如果继续保存会生成同名文件，因此无法继续覆盖保存，所以会出现保存失败的情况。如果您遇到这种情况，请将之前的模型结果文件关闭，并修改文件名（如加入后缀等），然后再点击“结果保存”键。
- 如果您在使用中出现了什么问题，请及时联系我的邮件，也欢迎您对后续的功能进行建议 <i class="fa-regular fa-envelope"></i>
- 解释权归作者所有 <i class="fa-regular fa-face-smile-wink"></i>  

### 软件激活
<i class="fa-solid fa-battery-empty"></i>  目前试用版本会内置`License`，为功能限制的版本，提供了限期内的普通效率模型的测算  
<i class="fa-solid fa-battery-full"></i>  `License`分为三种，第一种是普通模型测算，第二种是普通模型测算+超效率模型测算，第三种是全功能解锁，包括普通模型测算+超效率模型测算+Malmquist指数模型测算，以上三种均可以计算包含非期望产出的相关模型，并享受版本更新的服务    
<i class="fa-solid fa-compass"></i>   如果您需要使用超效率模型与Malmquist模型，请及时联系我，我将为您提供`License`以及激活方法  
<i class="fa-solid fa-circle-right"></i>  如果您已经获取了`License`，在版本更新时，请备份好`License`，即把license先移到别的文件夹，安装好新版本后再移回    


**Note**：软件内置的求解器采用的是当今学业与业界评价十分高的开源求解器，本软件基于此求解器进行算法代码的书写，足以解决中小规模的`DEA问题`，且求解速度十分快。由于目前软件的算法实现部分与界面开发功能均由一人完成，难免会出现一些bug <i class="fa-regular fa-face-sad-tear"></i> ，如果您在体验过程中遇到了问题，或者发现计算结果有误，欢迎及时联系我！

### 结语
<i class="fa-solid fa-award"></i>  大家有什么想法的话，欢迎联系我！如果您有一定的开发经验，也可以联系我，谢谢大家~

### Support or Contact
<i class="fa-brands fa-qq"></i> QQ：:(fas fa-address-card): 2229263318
<a target="_blank" href="http://wpa.qq.com/msgrd?v=3&uin=2229263318&site=qq&menu=yes"><img border="0" src="http://wpa.qq.com/pa?p=2:2229263318:41" alt="点击这里给我发消息" title="点击这里给我发消息"/></a>

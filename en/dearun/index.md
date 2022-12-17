# Introdution to Dearun


<script src="https://kit.fontawesome.com/5519c56e9e.js" crossorigin="anonymous"></script>
<script src="https://assets.salesmartly.com/js/project_3040_3314_1657543658.js"></script>
## 1 Software Description  
&nbsp;&nbsp;&nbsp;&nbsp;<i class="fa-brands fa-fly"></i> Data envelopment analysis (DEA) is a non parametric method to evaluate the relative effectiveness of decision making units (DMUs) with multiple inputs and outputs. It does not need to give weights and hypothetical distributions in advance, and can directly determine the structure of the production frontier through input and output data. As a cross field of mathematics, operations research and computer science, DEA method has been widely used in many fields.  

&nbsp;&nbsp;&nbsp;&nbsp;<i class="fa-solid fa-book-bookmark"></i>  Most researchers who are new to DEA will probably have deep doubts about this type of optimisation model and will not know where to start. If you want to thoroughly understand the mechanics of DEA models, you must master the knowledge of operational research, including how to build, solve and analyse optimisation models, which means a high learning cost. There are currently some software available on the market to handle DEA models, but the free software can only solve simple CCR/BCC models, which are simply not adequate for everyday research needs. This is the reason for the development of this software, which contains the current mainstream models in the field of DEA research, including basic efficiency models, super-efficiency models, network DEA models and dynamic Malmquist index analysis, and can handle situations where there are undesirable outputs. This article will introduce you to the installation and running process of **Dearun** software, so that you can get started with the software more quickly.

&nbsp;&nbsp;&nbsp;&nbsp;<i class="fa-solid fa-circle-right"></i>  If the current site is slow to access, or if some of the images do not load, please click on these sites:  [Alternative link 1](https://dearun.top/dearun/) &nbsp;
[Alternative link 2](https://dearun.buzz/dearun/)&nbsp;
[Alternative link 3](https://dearun.club/dearun/)    

&nbsp;&nbsp;&nbsp;&nbsp;> Dearun software latest version： **3.0.1**


## 2 Download and installation
> Dearun software is currently only available for 64-bit Windows systems and is not yet available for Mac.  
### Download

- Click here for Dearun installation file：<i class="fa-solid fa-file-zipper"></i> [Download link <i class="fa-solid fa-up-right-from-square"></i>](http://1.116.143.157/Dearun_Setup.exe)

{{< admonition type=failure title="Download failure solutions" open=true >}}
1. if the download link does not respond, please change your browser and try again.
2. If you are prompted with `Dearun_Setup.exe cannot be safely downloaded`, please right click on the prompt and select `Still Reserved` in the pop-up dialogue box to start the download.
{{< /admonition >}}

### Installation
- Please follow these steps to run Dearun:  
1. Click on the `Dearun_Setup.exe` file
<img src="\images\Dearun_Setup.png" width = "70" height = "70" alt="Image cannot be loaded" align=center /></img>
2. Please follow the installation steps, it is recommended to install on a non-system disk such as `D, E`.  
<img src="\images\安装步骤1.png"  width = "300" height = "200" alt="Image cannot be loaded" align=center /></img>  
<img src="\images\安装步骤2.png" width = "300" height = "200" alt="Image cannot be loaded" align=center /></img>

3. Double click to run `Dearun.exe` on the desktop  
<img src="\images\应用.png" width = "70" height = "70" alt="Image cannot be loaded" align=center /></img>

- **Note**：  If you are prompted that the license is expired, please download this file and copy it to the root directory of the software installation: ([Download link <i class="fa-solid fa-up-right-from-square"></i>](http://1.116.143.157/license.lic)).  
<img src="\images\许可安装en.png" width = "500" height = "300" alt="Image cannot be loaded" align=center /></img>  
- If you have done these steps correctly, the following screen will appear on your desktop:   

<img src="\images\Dearun展示图片.png" width = "550" height = "350" alt="Image cannot be loaded" align=center /></img>  

{{< admonition type=failure title="Software compatibility issues" open=true >}}
**If the software interface does not display properly, please refer to the software compatibility solutions at the bottom of the website.**    
[Solutions to software compatibility issues <i class="fa-solid fa-square-pen"></i>](../dearun/#5-software-compatibility-issues)  {{< version 2.1.7>}}
{{< /admonition >}}


## 3 Dearun Features

<i class="fa-solid fa-compass"></i> Congratulations! you have successfully opened Dearun and will be introduced to the functions of the software:  
- Calculation of efficiency values for conventional Radial (CCR, BCC), SBM, WSBM, DDF, EBM, MinDP (minimum distance to frontier), Directional SBM, Non-radial DDF models 
- Calculation of efficiency value for FDH model
- Six mainstream cross-efficiency models can be calculated 
- Pessimistic input oriented CCR model,output oriented CCR model, SBM model  
- ZSG-DEA model
- Calculation of super-efficiency values for conventional Radial, SBM, DDF, EBM and Directional SBM models
- handle cases that include undesirable outputs (except for EBM models)
- Different returns to scale assumptions can be chosen for the above models: CRS (constant returns to scale), VRS (variable returns to scale)
- Calculate **adjacent** or **global** Malmquist index for CCR, SBM, SBM super-efficiency, DDF, EBM based on  and decompose into technological change and efficiency change
- Calculation of ML index and GML index models
- Calculation of the global Malmquist Luenberger Index and global Luenberger Index for  Directional SBM model, Non-radial DDF model。
- Calculation of windows DEA model with customizable window periods
- Calculation of Meta-frontier model 
- Calculation of various basic two-stage network DEA models (including inputs, shared inputs, intermediate products, outputs)
- No additional installation of lower versions of Excel, good compatibility

## 4 Software License
<i class="fa-solid fa-battery-empty"></i>  The direct download version is Dearun Trial {{< version 2.1.7>}}，which is a functionally limited version, provides the following general efficiency models:
1. input and output oriented CCR, BCC models
2. non-radial SBM model (include undesirable output)
3. input and output oriented CCR, BCC super-efficiency models
4. Meta-frontier CCR, BCC, SBM models
5. Global or adjacent Malmquist index for input and output oriented CCR, BCC models
6. Global Malmquist index for SBM models 
7. Global Meta-frontier CCR, BCC, SBM Malmuqist index  
8. Two-stage network DEA model  

## 5 Software compatibility issues
<img src="\images\兼容性问题1.png" width = "550" height = "600" alt="Image cannot be loaded" align=center /></img>   

## 6 Concluding remarks
The software's built-in solver is an open source solver that is highly regarded by academics and the industry. The algorithm code is based on this solver and is sufficient to solve small to medium sized data set. As the algorithm implementation part of the software and the interface development function are both done by one person, some bugs will inevitably occur <i class="fa-regular fa-face-sad-tear"></i>.

If you encounter problems during your experience, or find errors in the calculations, please do not hesitate to contact me!  


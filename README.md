# DicomNotes
Dicom学习应用笔记

接触Dicom以来，感觉它的学习成本很高，目前也只是因为业务需要对其进行了一点点的学习，毕竟如果不去对它进行了解，业务的实现就无从下手。

Dicom的资料并不多，还大部分是英文，找资料的时候发现一个前辈对dicom协议进行了翻译工作，

地址 https://github.com/zssure-thu/DICOM-Chinese

### 基本流程

1. Modality worklist
2. Modality performed procedure step
3. Storage Commitment
4. Instance availability notification

目前主要使用的 Dicom 开发包有：

### Dcmtk 
该开源项目由德国offis公司开发，经过十几年的开发维护，已经基本实现了dicom协议的所有内容，

它只提供静态库链接和.exe程序，二次开发后才能进行更灵活的应用。
* 主要开发语言：C、C++
* 支持平台：Linux、Windows、MacOS…，使用CMake编译处理后，几乎可以支持所有平台
* 主页：http://dicom.offis.de 
* 下载：http://dicom.offis.de/dcmtk.php.en 
* 论坛：http://forum.dcmtk.org/ 

### mDCM (fo-dicom)
mDCM基于Dcmtk开发，fo-dicom是mDCM的升级版本，

它使用C#对Dcmtk进行了封装，Windows平台大多使用该库。

* 地址：https://github.com/ignacioinnovo/mdcm
       https://github.com/fo-dicom/fo-dicom

### DCM4CHE
采用Java开发
* 地址：https://www.dcm4che.org

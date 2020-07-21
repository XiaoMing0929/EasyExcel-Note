# EasyExcel

> 本篇博客博涵

## 概述：

### 1.为什么要使用EasyExcel?

> EasyExcel是一个基于Java的简单、省内存的读写Excel的开源项目，在尽可能节约内存的情况下支持读写百M的Excel。
>
> Java解析、生成Excel比较有名的框架有Apache poi、jxl。但他们都存在一个严重的问题就是非常的耗内存，poi有一套SAX模式的API可以一定程度的解决一些内存溢出的问题，但POI还是有一些缺陷，比如07版Excel解压缩以及解压后存储都是在内存中完成的，内存消耗依然很大。easyexcel重写了poi对07版Excel的解析，能够原本一个3M的excel用POI sax依然需要100M左右内存降低到几M，并且再大的excel不会出现内存溢出，03版依赖POI的sax模式。在上层做了模型转换的封装，让使用者使用更加简单方便。

> GitHub地址：https://github.com/alibaba/easyexcel

### 2.相关依赖：

```xml
<!-- https://mvnrepository.com/artifact/com.alibaba/easyexcel -->
<dependency>
    <groupId>com.alibaba</groupId>
    <artifactId>easyexcel</artifactId>
    <version>2.2.6</version>
</dependency>
```

## 写

1.最简单的写

2.根据参数只导出指定列

3.指定写入的列

4.复杂头写入

5.重复多次写入(写入单个或者多个sheet)

6.日期、数字或者自定义格式转换

7.图片导出

8.根据模板写入

9.列宽、行高

10.注解形式自定义样式

11.自定义样式

12.合并单元格

13.使用table取写入

14.动态头、实时生成头写入

15.自动列宽(不太精确)

16.自定义拦截器

## 读
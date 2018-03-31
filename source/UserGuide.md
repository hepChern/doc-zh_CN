# Guide for the users
## Warning
This is the very first version of Chern software. It will change a lot during its development. And I am not sure that it will be back compatiable.

## Startup
在安装好Chern之后，直接使用chen命令就可以新建一个项目。
Chern init可以从已有的Chern项目中新建。
随后就会进入ipython交互环境。可以作为shell使用。

## Basic element
### VTask
### VAlgorithm
### VData
### VDirectory

## 基本操作

### 目录操作
#### cd DESTINATION/OBJECT
将当前路径更改为DESTINATION/OBJECT，可以为路径，算法或任务等。

#### ls
查看当前OBJECT的信息

#### mv SOURCE DESTINATION
将`object`SOURCE移动到`object`DESTINATION。
如果DESTINATION是一个已有的路径，那么将SOURCE移动到DESTINATION下。
此操作会保持`impression`。

#### cp SOURCE DESTINATION
将`object`SOURCE复制到`object`DESTINATION。

#### rm SOURCE
删除`object`SOURCE

#### mkdir OBJECT
新建目录

#### mkalgorithm OBJECT
新建算法

#### mktask OBJECT
新建任务

### 算法/任务操作

#### status
查询该算法状态

#### jobs
查询全部作业

### 算法操作
#### add source

+ add input [input_data] [nickname]
+ add output [output_data] [nickname]
+ add algorithm [algorithm]
+ add rawdata [position]
+ add site [sitename]

### readme
+ readme edit

### 

## 批量模式
### 目录操作
#### obj("SOURCE").mv("DESTINATION")
+ 例子：
```
for source in ["file1", "file2", "file3", "file4"]:
  obj(source).move("..{}".format(source))
```



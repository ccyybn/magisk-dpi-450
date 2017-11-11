# 这是一个简单的Magisk模块示例

## module.prop
模块的基本信息文件

## config.sh
模块的配置文件，主要参数：

### AUTOMOUNT=false
Set to true if you need to enable Magic Mount
Most mods would like it to be enabled

### PROPFILE=true
Set to true if you need to load system.prop

### POSTFSDATA=false
Set to true if you need post-fs-data script

### LATESTARTSERVICE=false
Set to true if you need late_start service script

## system
这里面的文件和文件夹，会挂载到系统system目录，用来修改系统system目录

## common
### post-fs-data.sh
开机时在挂载各个模块之前执行

### service.sh
挂载好模块，启用magisk hide后执行

### system.prop
修改系统build.prop

## META-INF
默认脚本，不用改

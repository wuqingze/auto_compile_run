### 介绍
---------------
auto_compile_run 是一个能够实时检测代码变化自动执行编译运行的脚本程序。

开发过程中修改完代码、编译、运行，这个过程是重复的，因为保证一次编写出正确的代码似乎并不现实，实际情况是需要多次修改、编译、运行代码以保证正确的结果。那么基于这个场景，如果存在一个自动检测文本变化然后完成上诉过程的工具那么是不是很大成都提升了编码的效率呢？

### quickstart
* 安装when-changed插件
```
pip install: https://github.com/joh/when-changed/archive/master.zip
```
* 在工作目录运行 `run.sh`脚本
* 运行`tail -30f log`命令

### 注意事项
* 运行run.sh脚本和查看日志在同一个shell窗口中
* 杀死监控进程使用 `ps auxw | grep when-changed | awk '{print $2}' | xargs kill` 命令

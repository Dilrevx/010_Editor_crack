Binary Templates
===

NAND `.bt` templates.

By 2025, built-in marketplace has no ubi scripts. So I wrote one.


## Template 开发注意事项

1. `.bt`  是脚本语言，用声明变量的方式标注当前文件指针处的类型；同事，也可以用 FSeek, FTell 跳转文件标注位置
2. 支持在声明 `typedef struct` 的时候，用 `<format, read>` 等 xml 关键字，重载字段和整个结构体的显示颜色和显示的 value（所有 format 回调都要等主脚本 EOF 之后执行，因而基本上不太能执行文件操作）
3. 编译器有 bug，line number 要 +1
4. 不支持 C++ 语法

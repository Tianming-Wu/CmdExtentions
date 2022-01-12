# CmdExtentions
A light, powerful (awa) C++ based extension library for Windows cmd. Work with Batch.

# Description
```
    整个初级应用系统会使用全英文，后续会利用系统API支持多语言工作。
由于暂无法通过c++操作cmd环境变量，系统提供文件操作，请自行使用for命令和echo命令将文件系统与环境变量进行对接。如果哪位大佬有好的想法欢迎告诉我……
    文件操作统一采用 -i和 -o进行。-i选项不能与 -o选项同时使用，如有需要请分两次执行。-i选项使用要求文件必须存在，且有权限进行读写，否则程序会退出并将ERRORLEVEL设置为1（注：这个是通过return实现的，并不是能操作环境变量……）。当前版本不会验证文件内容，请自行确保执行安全。
    初级系统不完全包含帮助文档。第一阶段开发完成（v1.1.0.0+）时，开放CmdExentions命令，可通过CmdExtentions -h 获取完整命令帮助列表。（计划中）
    现在是通过将句柄写入文件再从文件读取……并且窗口句柄是用的GetForegroundWindow();实现的……也是有想法告诉我awa
```

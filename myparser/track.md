# Macro parser


Condition:
-   All source files compile successfully.
-   All strings are ANSI encoded.

Suppose:
-   There are no identifiers with parameters.
-   There are no raw string.
-   All characters are ASCII characters.
-   There are no wstring concatenation.

## 读文件：

f.readline() -> str

f.read() -> str -> unicode

## remove comment

func(s): 

## 

skeleton

header: #*** 

identifier: word

others: constant

## constant

python -- c



## unecessary macro name 1/8

-   comment
-   #define kkk 
-   #undef jjj

去注释：
遇到字符串或字符，

处理分支：

首先记录每个if指令（#ifdef,#ifndef）的结尾（#endif），和可能存在分支（#else）
具体执行时遇到if指令时，根据判断的结果直接跳到其结尾或分支。

字符串常量中不能有换行符，以下不合法：
#define string_with_comment_symbol_1 "// /// 
////"
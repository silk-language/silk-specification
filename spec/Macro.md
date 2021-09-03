#Silk Macro Specification
***
## 1.lexer Macro
    规则：
        #lexer macro_name(token_list)
    说明：
        输入token_list,输出token_list
        用已经提供的语法实现一些自定义语法
        Token流后处理

## 2.syntax Macro
    规则：
        #syntax macro_name(ast)
    说明：
        输入ast,输出ast
        用已经提供的语法实现一些自定义语法
        ast后处理

## 3.类C宏
    规则：
        #define macro_name(arg1,arg2...argN)
    说明：
        
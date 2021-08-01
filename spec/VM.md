
## 虚拟机设计
    AST -> byte code -> 解释执行编译期部分 -> 根据byte code生成LLVM IR -> binary code gen

## 指令集
    * pushi (size,
    * pushui (size,)
    * pushf (size,)
    * popi (size,)
    * popui (size,)
    * pop (size,)
    
    *addi (size,)
    *addui(size,)
    *addf (size,)
    
    *callbuiltin ("name")
    * syscall
    
    
    
    
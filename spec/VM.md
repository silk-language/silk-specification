
## 虚拟机设计
    AST -> byte code -> 解释执行编译期部分 -> 根据byte code生成LLVM IR -> binary code gen

## 指令集
    *pushci8(variable_index,value)
    *pushci16(variable_index,value)
    *pushci32(variable_index,value)
    *pushci64(variable_index,value)
    *pushcui8(variable_index,value)
    *pushcui16(variable_index,value)
    *pushcui32(variable_index,value)
    *pushcui64(variable_index,value)
    *pushi8 (variable_index,value)
    *pushi16(variable_index,value)
    *pushi32(variable_index,value)
    *pushi64(variable_index,value)
    *pushui8(variable_index,value)
    *pushui16(variable_index,value)
    *pushui32(variable_index,value)
    *pushui64(variable_index,value)
    *pop [N]
    
    *addi8
    *addi16
    *addi32
    *addi64
    *addui8
    *addui16
    *addui32
    *addui64
    
    *callbuiltin ("name")
    *extern_v
    *callexternal 
    * syscall
    
    
    
    
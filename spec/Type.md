#Silk Type Specification

类型:一个类型就是一个集合，类型的实例就是集合的元素。

## 0、支持的操作
    +
    -
    *
    /
    ~
    %
    ^
    &

#逻辑运算
    * and
    
    * or
    
    * not
    

#类型描述符
    用于类型描述列表，是一类特殊函数，输入为类型，输出为bool
    内建：
        inheritable 可被继承
        sizeable 有尺寸的类型
        copyable 可复制
        
    自定义:
        type descriptor custome_desc(type A)
                        {
                          return hasattr(A,"xx")
                        }
##关键字
    
## 0、特殊类型
    
    sizeable type:
        * address type
                refer to a memory address, has no type
            
        * object type
            [inheritable,]
            
        * data type
            [inheritable,]
            can only contain base type and data type
            
        * traits type
            [inheritable,]
                interface
                
        * type type
                for every type,its type is type
    
    nonsizeable type:
        * nothing type
          can have only one value:None
    
## 一、 基础类型
    * 一阶类型
        * int8
            copyable memory object
            [-2^7,2^7-1]
        
        * int16
            copyable memory object
            [-2^15,2^15-1]
        
        * int32
            copyable memory object
            [-2^31,2^31-1]
        
        * int64
            copyable memory object
            [-2^63,2^63-1]
        
        * float
            copyable memory object
            IEEE 754 32bit float
        
        * double
            copyable memory object
            IEEE 754 64bit float
        
        * bool
            copyable memory object
            this type has two value:
            True logically True
            False logically False
        
        * char
            copyable memory object
            four byte unicode codepoint
            [0,2^32-1]
    
    * byte
    8 bit value
    [0,2^8-1]

## 二、复合类型
    复合类型是指由基础类型进行组合而得到的类型，其取值范围是其所组合类型的取值范围的笛卡尔积
    因此，复合类型
    
    * struct
    
    * array
        数组类型，由N个元素e1,e2,...en构成，取值范围为[type(e1)*type(e2)*...type(en)]
        因此，数组类型的构造有两个参数，N代表元素个数，以及可能的N个元素的类型
        比如：
            array<5,int8> a; 代表a有5个元素，每个元素的类型是int类型
            array<5,int8,int16,int32,bool,char> 代表a有5个元素，第一个元素的类型是5,第二个元素的类型是int8，以此类推
            
    
## 标准库
    * memory type
    data type
        start:address
        len:uint32
        alignment:uint16
        flags:uint32
    
    * ptr<T> pointer to T
        address:address_type
        only support index
        ptr<int> a=new int;
        ptr
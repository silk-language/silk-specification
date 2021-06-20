#Silk Token Specification
***
## 1.Identifier 标识符
    规则：
        Identifier = Silk_IDStart XID_Continue*
        Silk_IDStart = XID_Start|'_'
    说明：
        用来表示程序中的变量名，函数名，类名等等（不包括关键字）
        XID_Start XID_Continue 定义参考:http://www.unicode.org/Public/4.1.0/ucd/DerivedCoreProperties.txt

## 2.type 类型
    规则：
        type
    说明：
        关键字

## 3.struct 数据类
    规则：
        struct
    说明：
        关键字
        
## 4.enum 枚举
    规则：
        enum
    说明：
        关键字

## 5.int 整数
    规则：
        int8,int16,int32,int64
        uint8,uint16,uint32,uint64
    说明：
        关键字

## 6.float 单精度浮点数
    规则：
        float
    说明：
        关键字
## 7.double 双精度浮点数
    规则：
        double
    说明：
        关键字
        
## 8.str 字符串
    规则：
        str
    说明：
        关键字
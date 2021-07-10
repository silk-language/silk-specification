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
        ""单行字符串常量
        ''' '''多行字符串常量
    说明：
        关键字

## 9.bool 布尔类型
    规则：
        bool
    说明：
        关键字

## 10 浮点字面值
    规则:
        Digit+ . Digit+ [decimal_exponent]
                Digit 如下:
                    0 1 2 3 4 5 6 7 8 9
                decimal_exponent 如下:
                    e | E [exponent_sign] Digit+
                exponent_sign 如下:
                    +|-

## 11 整数字面值
    规则:
        decimal_literal :
            NoneZeroDigit Digit*
        hex_literal :
            0x|0X HexDigit+
        binary_literal
            0b|0B BinDigit+
        
        NoneZeroDigit 如下:
            1, 2, 3, 4, 5, 6, 7, 8, 9
        Digit 如下:
            0 1 2 3 4 5 6 7 8 9
        HexDigit 如下:
            0, 1, 2, 3, 4, 5, 6, 7, 8, 9, a, A, b, B, c, C, d, D, e, E, f, F
        BinDigit 如下:
            0 1
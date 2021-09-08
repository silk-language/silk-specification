
import package.sub_package.module
import package.sub_package.module as alias_name
from package.sub_package.module import name
from package import package
from package.sub_package import module

enum A
{
    
}


struct B
{
    [property_meta1,property_meta2]
    int x;
    [property_meta1,property_meta2]
    int y;
}

@class_decorator1
@class_decorator2
class C(object)
{
    public:
    
    private:
    
}

@decorator1
@decorator2
[tag1,tag2,tag...N]
func print([NonNegative,Odd] int x,[NonNull,lambda s:MaxLen(s,7)] str y)->[Even,Negative]int
{
    @line_decorator
    int i=1,j=10;
    
}
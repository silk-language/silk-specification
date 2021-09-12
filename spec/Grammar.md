
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

decorator hook
descriptor metadata
validator validate
validator odd_validate(int x)
{
    if(x%2==0)
    {
        return true;
    }
    
    return false;
}


@decorator1
@decorator2
[tag1,tag2,tag...N]
func print(int x[NonNegative,Odd], str y [NonNull,lambda s:MaxLen(s,7)])->int[Even,Negative]
{
    @line_decorator
    {
        int i=1,j=10;
        int v[odd_validator]=get_odd();
        (i,j)[odd_validator];
        
    }
    
    with []
    
}
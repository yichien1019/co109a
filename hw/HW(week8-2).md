# 第八週補充習題 -- 撰寫組合語言
## C語言code:
```
#include <stdio.h>
/*while(1)
{
    R0=R0+1
}*/
int main(){
    R0=1
    while(1)
    {
        R0=R0+1
    }
}
```
## .asm:
```

@0
M=1
@0
M=M+1
@2
0;JMP
```
## pictuure:
![image](https://github.com/yichien1019/co109a/blob/master/hw/8-2.png) 




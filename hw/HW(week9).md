# 第九週習題 -- 第四章第一題 Mult.asm
## Mult.asm:
[mult.asm](https://github.com/yichien1019/co109a/blob/master/04/mult/mult.asm)
#### code:
```
// This file is part of www.nand2tetris.org
// and the book "The Elements of Computing Systems"
// by Nisan and Schocken, MIT Press.
// File name: projects/04/Mult.asm

// Multiplies R0 and R1 and stores the result in R2.
// (R0, R1, R2 refer to RAM[0], RAM[1], and RAM[2], respectively.)

// Put your code here.
@0
D=A //先將D設0
@2  
M=D //將結果先規0
@0  //LOOP1
D=M //將R0設為計數器
@16
D;JLE //D等於0跳出迴圈
@1
D=M  //將值輸入D
@2
M=D+M //將D值加入R2
@0
M=M-1 //計數器-1
@4  
0;JMP //回到LOOP1
@16
0;JMP
```

## hack:
#### picture:
![image](https://github.com/yichien1019/co109a/blob/master/hw/9-1.jpg?raw=true) 

## result:
#### picture:
![image](https://github.com/yichien1019/co109a/blob/master/hw/9-2.jpg?raw=true) 

![image](https://github.com/yichien1019/co109a/blob/master/hw/9-3.jpg?raw=true) 


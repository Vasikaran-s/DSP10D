# DSP-10-D



#ADDITION USING INDIRECT ADDRESSSING MODE

PROGRAM:
 .mmregs 
.text 
START: 
LD #00H,A 
STM #1000H,AR4 
STM #2000H,AR5 
STM #3000H,AR6 
LD *AR4,A 
ADD *AR5,A 
STL A,*AR6+ 
HLT: B HLT  
 
 
INPUT: 
 
DATA MEMORY: 
 
1000h 0002 
2000h 0004 
 
OUTPUT: 
 
DATA MEMORY: 
 
3000h 0006 
 
 
 
 
 
 
 
 
 

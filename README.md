// an 10 bit counter 
module counter (clear , clock , count):
parameter N = 10
input clear,clock;
output[0:9] count ; reg[0:9] count;

always @(negedge clock)
if (clear)
count <= 0;
else
count <= count + 1;
endmudule 

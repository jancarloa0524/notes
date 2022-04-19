[jsbin]()

In order to understand bitwise operators, first, understand binary!

Binary is a base-2 number system, 0 and 1. So, it would count something like this. From 0-10, you would say:
- 0: 0
- 1: 1
- 10: 2
- 11: 3
- 100: 4
- 101: 5
- 110: 6
- 111: 7
- 1000: 8
- 1001: 9

You basically move the 1 over, until all of it is 1, in which case you have to update the number of bits by 1. You see this happen at the integers 2, 4, 8, 16, 32, etc. This follows an increase by a factor of 2, 2^1, 2^2, 2^3, 2^4, 2^5, etc. 

- 1; 2^0; 1
- 2; 2^1; 10
- 4; 2^2; 100
- 8; 2^3; 1000
- 16; 2^4; 10000
- 32; 2^5; 100000
- 64; 2^6; 1000000
- 128; 2^7; 10000000
- And so on

Notice: with each increase, the number of 0's corresponds to the exponent. 
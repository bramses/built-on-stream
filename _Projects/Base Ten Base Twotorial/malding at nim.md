# malding at nim

#basetwotorial

- [nim](https://www.cut-the-knot.org/nim_st.shtml) is based on boolean arithmetic 
	- relies on XOR => 0x0 = 0, 0x1=1, 1x0=1, 1x1=0[^1]
	- the goal is to never let the computer get the initiative from the player

is 111 == 1111111?^[no, its 127]

1100^0111^0100=1111


1. 4095 - (xor of other two rows)
2. 1111111^0001111 = 1110000 = 112
3. 4095 - 112 = 3983

1. 1111 ^ 1000 = 0111 = 7
2. 31 - 7 = 24 = 11000

1. 100 ^ 111 = 011 = 3
2. 3 - 3 = 0


[^1]: XOR applies bitwise to the binary representation of two or more numbers. 
	For example, if x=7 and y=11 are two decimal numbers then their binary representations will be  (x)2=111 and (y)2=1011, respectively. 
	Therefore, x ^ y = 1100.
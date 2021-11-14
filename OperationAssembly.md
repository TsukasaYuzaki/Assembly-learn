# not
Not: inverts the bit

not

rax = 11111

not rax

=> rax - 00000

# Xor 

a = 101

b = 110

xor a, b

a = 010

# and

and: opposite from xor

a = 110

b = 101

and a, b

a = 100

# Test:

The TEST instruction works same as the AND operation, but unlike AND instruction, it does not change the first operand.

test al, 0x1

jz _somewhere

# Or:

rax = 10101

rbx = 11010

Or rax, rbx

rax = 11111




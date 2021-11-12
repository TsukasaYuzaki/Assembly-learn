# Assembly-learn

![alt_text](https://media.cheggcdn.com/media%2F915%2F9152d5e6-6c17-4e93-aa8d-d70b5507d021%2Fphpgt9SZU.png)

a. uint32_t add32(uint32_t x, uint32_t y) // returns (x+y)%(2^32); any carry out is lost

b. uint64_t add32_64(uint32_t x, uint32_t y) // returns x+y; sum contains any carry

c. uint64_t add64(uint64_t x, uint64_t y) // returns (x+y)%(2^64)

d. uint32_t shiftLeftU32 (uint32_t x, uint32_t p) // returns x << p = x*2^p for p = 0..31

e. uint32_t shiftU32(uint32_t x, int32_t p) // return x*2^p for p = -31..31

f. int32_t shiftLeftS32 (int32_t x, uint32_t p) // returns x << p = x*2^p for p = 0..31

g. int32_t shiftS32(int32_t x, int32_t p) // return x*2^p for p = -31..31

h. uint32_t isEqual32(uint32_t x, uint32_t y) // returns 1 if x=y, 0 if x!=y

i. int32_t isEqual32(int32_t x, int32_t y) // returns 1 if x=y, 0 if x!=y

j. uint32_t isEven(uint32_t x) // returns 1 if even, 0 if not even

k. uint32_t maxU32(uint32_t x, uint32_t y) // returns the maximum of x, y

l. int32_t maxS32(int32_t x, int32_t y) // returns the maximum of x, y


![alt_text](https://i.imgur.com/km2o5yX.png)


-setb: set if below, use after cmp Ex: setb al set al to 1

pshufb:
SHUFFLE =  0x000D0C0A08040F030E090B0501070602
s1 = [BitVec("x%i" % i, 8) for i in range(16)]
s2 = []

for i in range(16):
	idx = (SHUFFLE >> (i * 8)) & 255
	s2.append(s1[idx])
  
 s1: create x1, x2, x3...
 s2: create the pshufb version of s1


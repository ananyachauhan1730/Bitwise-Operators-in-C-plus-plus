# Bitwise-Operators-in-C-plus-plus
Aim: To study and implement C++ Bitwise Operators

Tool: VS Code

Theory: 
Bitwise operators directly perform operations on binary representations of integers. These operators manipulate individual bits of data, enabling efficient computation especially useful in low-level programming, optimization, and hardware-level tasks. The two provided programs demonstrate bitwise manipulation using various operators.

1.Basic Bitwise Operations:

•AND (&): Compares each bit of two numbers and returns 1 only if both bits are 1.
•OR (|): Compares each bit and returns 1 if either of the bits is 1.
•NOT (~): Inverts each bit of the number, turning 1 into 0 and 0 into 1, also known as complement.
•XOR (^): Returns 1 if the corresponding bits of operands are different. 
•Left Shift (<<): Shifts bits of a number to the left, effectively 
multiplying the number by powers of 2. 
•Right Shift (>>): Shifts bits to the right, effectively dividing the number by powers of 2.

2.Bit Manipulation (Setting and Resetting Bits)

•Setting a Bit: To set (turn on) a particular bit, the program uses OR (|) with a left-shifted mask where the desired bit is set to 1. This ensures that the target bit is set without affecting other bits.

•Resetting a Bit: To reset (turn off) a bit, the program uses AND (&) with the complement of the left-shifted mask, ensuring only the targeted bit is cleared.

1. Program 1 Algorithm:

Step 1: What Are Bitwise Operators?

Bitwise operators perform operations on the binary bits of integer values.

Each integer is stored in memory as a sequence of bits (0s and 1s).

Bitwise operators manipulate these bits directly.

Step 2: How Bitwise Operators Work.

Imagine two integers represented in binary:

Example: a = 5 is 0101 in 4-bit binary.

Example: b = 9 is 1001 in 4-bit binary.

1.AND (&):

Compare each bit of a and b.

Only when both bits are 1, the result bit is 1.

Example: 0101 & 1001 = 0001

2.OR (|):

Compare each bit of a and b.

If any bit is 1, result bit is 1.

Example: 0101 | 1001 = 1101

3.XOR (^):

Result bit is 1 if bits differ.

Example: 0101 ^ 1001 = 1100

4.NOT (~):

Flips all bits of the number.

If a = 0101, ~a = 1010.

For signed integers, this also changes the sign due to two’s complement representation.

5.Left Shift (<<):

Moves bits to the left, adding zeros on the right.

Each shift multiplies the number by 2.

Example: 0101 << 1 = 1010

6.Right Shift (>>):

Moves bits to the right.

Each shift divides the number by 2 (integer division).

For unsigned numbers, zeros fill the left bits.

For signed numbers, sign bit (0 or 1) might fill the left (arithmetic shift).

Step 4: Why Use Bitwise Operators?
Bitwise operations are very fast because they work at the hardware level.

Used in:

Low-level programming (e.g., device drivers, embedded systems)

Manipulating flags and masks

Efficient arithmetic operations (like multiplication/division by powers of 2)

Cryptography, compression algorithms, graphics

Step 5: Important Notes
Bitwise NOT (~) behaves differently from logical NOT (!) — it flips bits, not just true/false.

Be aware of signed vs unsigned integers when using right shift and NOT.

Bitwise operations only work on integral types (int, char, long, etc.).

conclusion:

Bitwise operators in C++ provide a powerful and efficient way to manipulate individual bits within integer data types. Understanding these operators allows you to perform low-level data processing tasks such as setting, clearing, toggling bits, and optimizing arithmetic operations. Mastery of bitwise operations is essential in systems programming, embedded development, and applications requiring high-performance computation. However, careful attention must be paid to data types and signedness, especially when using operators like NOT (~) and right shift (>>), to avoid unexpected results.





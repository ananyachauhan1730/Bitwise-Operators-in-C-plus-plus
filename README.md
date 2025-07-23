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

Start Initialize integers a = 13, b = 14 Perform and store results of: a & b → AND a | b → OR ~a and ~b → NOT a ^ b → XOR a << 1, b << 1 → Left Shift a >> 1, b >> 1 → Right Shift Print all results End

2. Program 2: Bit Set and Reset Algorithm:

Start Initialize integer a = 230 Input bit position to set → bit_set Set bit using a | (1 << bit_set) Input bit position to reset → bit_reset Reset bit using a & (~(1 << bit_reset)) Print results of both operations End

Conclusion: Hence, we performed the Bitwise Operations on numbers given as input and we have reset and set the given digits of a binary number.

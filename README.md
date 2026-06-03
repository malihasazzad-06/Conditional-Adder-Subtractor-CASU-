# Conditional-Adder-Subtractor-CASU-

Description

The CASU is a 3-bit combinational logic circuit that performs different operations based on input comparison:

* If A = B → outputs A + B
* If A ≠ B → outputs |A − B|

Working

1. Equality check: Uses XNOR gates to compare each bit of A and B.
    * If all bits match → A = B
    * Otherwise → A ≠ B
2. Operation selection:
    * Equal → 3-bit binary addition
    * Not equal → absolute difference using subtraction logic
3. Final output: Selected using basic gate-based multiplexer logic.

Gates Used

AND, OR, NOT, NAND, NOR, XOR, XNOR

Examples

Input:
A = 010, B = 010
Output: 100 (2 + 2 = 4)

Input:
A = 011, B = 101
Output: 010 (|3 − 5| = 2)

COMPUTER ARCHITECTURE – PYTHON PROGRAMS

Question 1: Effective Address Calculation

Aim

To write a Python program to calculate the effective address using different addressing modes.

Description

This program calculates the operand or effective address using four addressing modes:

1. Immediate Addressing
2. Direct Addressing
3. Indirect Addressing
4. Indexed Addressing

Given Values

- Address field = 200
- Register R1 = 40
- Memory[200] = 500
- Memory[240] = 900
- Immediate operand = 25

Rules Used

- Immediate: Operand = Given value
- Direct: EA = Address field
- Indirect: EA = Memory[Address field]
- Indexed: EA = Address field + Register R1

Expected Output

Immediate Addressing:
Operand = 25

Direct Addressing:
Effective Address = 200
Operand = 500

Indirect Addressing:
Effective Address = 500
Operand = Not available

Indexed Addressing:
Effective Address = 240
Operand = 900

Result

The Python program successfully calculates the effective address and operand for all four addressing modes.

---

Question 2: Virtual to Physical Address Translation

Aim

To write a Python program to translate virtual addresses into physical addresses using a page table.

Description

This program converts virtual addresses into physical addresses using paging. It calculates the virtual page number and offset, checks the page table and identifies page faults.

Given Values

- Page size = 1024 bytes
- Virtual Page 0 → Frame 5
- Virtual Page 1 → Frame 2
- Virtual Page 2 → Not Present
- Virtual Page 3 → Frame 7

Formula

- Page Number = Virtual Address // Page Size
- Offset = Virtual Address % Page Size
- Physical Address = (Frame Number × Page Size) + Offset

Virtual Addresses

500, 1500, 2500 and 3500.

Expected Output

Virtual Address | Page | Offset | Frame | Physical Address
500  | 0 | 500 | 5 | 5620
1500 | 1 | 476 | 2 | 2524
2500 | 2 | 452 | Page Fault | Page Fault
3500 | 3 | 428 | 7 | 7596

Result

The Python program successfully translates virtual addresses into physical addresses using the page table and identifies page faults when a page is not present.

---

Conclusion

Both Python programs demonstrate important concepts of Computer Architecture, including addressing modes, effective address calculation, paging and virtual-to-physical address translation.# computer_architecture_assignment
Assignment-Effective address calculation and virtual to physical address calculations

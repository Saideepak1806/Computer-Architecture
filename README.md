# Computer Architecture - Assembly Language Experiments

This repository contains a comprehensive collection of **8086 and 8085 assembly language experiments** demonstrating fundamental concepts in computer architecture, digital logic, and low-level programming.

## 📋 Repository Overview

This project explores core concepts of computer architecture through practical assembly language implementations, covering:
- **Arithmetic Operations** (Addition, Subtraction, Multiplication, Division)
- **Number Systems & Representations** (Complements, Decimal to Hexadecimal)
- **Logical Circuits** (Half Adder, Full Adder, Half Subtractor, Full Subtractor)
- **Sorting Algorithms** (Ascending, Descending Order)
- **Array Operations** (Finding Largest, Smallest, GCD, LCM)
- **Mathematical Operations** (Factorial, ODD/EVEN, Comparisons)
- **Basic Control Flow** (If-Else Logic)

---

## 🔢 Experiments by Category

### 1. **Number System & Representations**

#### 1'S COMPLIMENT
- **Concept**: One's complement representation for negative numbers in binary
- **Implementation**: Demonstrates how to calculate one's complement by inverting all bits
- **Use Case**: Understanding signed number representation in early computer systems

#### 2'S COMPLIMENT
- **Concept**: Two's complement representation (modern standard for negative numbers)
- **Implementation**: Shows the process of inverting bits and adding 1 to get two's complement
- **Use Case**: This is the standard method used in modern processors for representing negative integers

#### DECIMAL TO HEXA
- **Concept**: Converting decimal numbers to hexadecimal representation
- **Implementation**: Assembly code to perform base-10 to base-16 conversion
- **Use Case**: Understanding number system conversions essential for low-level programming and debugging

---

### 2. **Basic Arithmetic Operations - 8-bit**

#### 8BIT ADDITION
- **Concept**: Adding two 8-bit unsigned integers
- **Implementation**: Uses ADD instruction with carry flag handling
- **Learning**: Understanding register operations and carry propagation

#### 8BIT SUBTRACTION
- **Concept**: Subtracting one 8-bit number from another
- **Implementation**: Uses SUB instruction with borrow handling
- **Learning**: Signed and unsigned subtraction techniques

#### 8BIT MULTIPLICATION
- **Concept**: Multiplying two 8-bit unsigned numbers
- **Implementation**: Uses MUL instruction generating 16-bit result
- **Learning**: Product overflow and multi-register operations

#### 8BIT DIVISION
- **Concept**: Dividing two 8-bit unsigned numbers
- **Implementation**: Uses DIV instruction for quotient and remainder
- **Learning**: Understanding division operation and remainder calculation

---

### 3. **16-bit Arithmetic Operations**

#### 16 BIT ADDITION
- **Concept**: Adding two 16-bit numbers with proper carry handling
- **Implementation**: Multi-byte addition with carry propagation
- **Use Case**: Extended precision arithmetic

#### 16 BIT ADDITION 8086
- **Concept**: 16-bit addition optimized for 8086 processor
- **Learning**: Processor-specific optimizations and instruction sets

#### 16 BIT SUBTRACTION
- **Concept**: Subtracting two 16-bit numbers
- **Implementation**: Handling borrow across 16-bit boundaries

#### 16 BIT SUBTRACTION 8086
- **Concept**: 16-bit subtraction with 8086 architecture considerations

#### 16 BIT MULTIPLICATION
- **Concept**: Multiplying two 16-bit unsigned numbers (result up to 32-bit)
- **Learning**: Extended multiplication and accumulator usage

#### 16 BIT MULTILICATION 8086
- **Concept**: 16-bit multiplication optimized for 8086 processor

#### 16 BIT DIVISION
- **Concept**: Dividing two 16-bit numbers
- **Implementation**: Using DIV instruction for 32-bit ÷ 16-bit operation

#### 16 BIT DIVISION 8086
- **Concept**: 16-bit division with 8086-specific optimizations

---

### 4. **Digital Logic Circuits - Adders & Subtractors**

#### Half Adder
- **Concept**: Basic combinational circuit that adds two single-bit inputs
- **Truth Table**: 
  - Inputs: A, B (1-bit each)
  - Outputs: Sum, Carry
- **Logic**: SUM = A XOR B, CARRY = A AND B
- **Application**: Building block for more complex arithmetic circuits

#### Full Adder
- **Concept**: Combinational circuit that adds three bits (including carry-in)
- **Truth Table**:
  - Inputs: A, B, Carry_in (1-bit each)
  - Outputs: Sum, Carry_out
- **Logic**: 
  - SUM = A XOR B XOR Carry_in
  - CARRY_OUT = (A AND B) OR (B AND Carry_in) OR (A AND Carry_in)
- **Application**: Used in cascaded form for multi-bit addition

#### Half Subtractor
- **Concept**: Basic combinational circuit that subtracts one single-bit from another
- **Logic**: DIFF = A XOR B, BORROW = NOT(A) AND B
- **Application**: Foundation for building larger subtraction circuits

#### Full Subtractor
- **Concept**: Combinational circuit that performs subtraction of three bits (with borrow-in)
- **Truth Table**:
  - Inputs: A, B, Borrow_in
  - Outputs: Difference, Borrow_out
- **Application**: Cascaded for multi-bit subtraction operations

---

### 5. **Array Operations**

#### LARGEST NUMBER IN ARRAY
- **Concept**: Iterating through an array to find the maximum value
- **Algorithm**: Compare each element with current maximum, update if larger
- **Learning**: Loop structures and conditional branching in assembly

#### SMALLEST NUMBER IN ARRAY
- **Concept**: Iterating through an array to find the minimum value
- **Algorithm**: Compare each element with current minimum, update if smaller
- **Learning**: Reverse comparison logic and array indexing

#### GREATEST OF 2 NOS
- **Concept**: Simple comparison to find larger of two numbers
- **Implementation**: Compare instruction followed by conditional jump
- **Learning**: Basic conditional logic

#### SMALLEST OF 2 NOS
- **Concept**: Simple comparison to find smaller of two numbers
- **Implementation**: Comparison with alternate branching logic

---

### 6. **Mathematical Operations**

#### ODD or EVEN
- **Concept**: Determining if a number is odd or even
- **Implementation**: Check LSB using AND with 1 or modulo operation
- **Learning**: Bitwise operations and their practical applications

#### POSITIVE AND NEGATIVE
- **Concept**: Determining the sign of a number
- **Implementation**: Check MSB (most significant bit) for sign in two's complement
- **Learning**: Understanding sign bit and number representation

#### FACTORIAL
- **Concept**: Computing n! (product of all positive integers up to n)
- **Implementation**: Loop-based multiplication from 1 to n
- **Learning**: Looping structures and accumulator operations

#### GCD (Greatest Common Divisor)
- **Concept**: Finding the GCD of two numbers using Euclidean algorithm
- **Algorithm**: Repeatedly replace larger number with remainder of division
- **Learning**: Iterative algorithms and modulo operations

#### LCM (Least Common Multiple)
- **Concept**: Finding the LCM of two numbers
- **Algorithm**: LCM(a, b) = (a × b) / GCD(a, b)
- **Learning**: Using previously computed GCD to calculate LCM

---

### 7. **Sorting Algorithms**

#### ASCENDING ORDER
- **Concept**: Arranging array elements in increasing order
- **Implementation**: Bubble sort or similar comparison-based sorting
- **Learning**: Nested loops, multiple comparisons, and array manipulation

#### DESCENDING ORDER
- **Concept**: Arranging array elements in decreasing order
- **Implementation**: Reverse comparison logic for sorting
- **Learning**: Loop control and reverse ordering logic

---

## 🎯 Key Learning Outcomes

By studying these experiments, you will understand:

1. **Low-Level Programming**: Direct CPU instruction usage and register manipulation
2. **Number Systems**: Binary, decimal, hexadecimal, and complement representations
3. **Arithmetic Operations**: How processors perform addition, subtraction, multiplication, and division
4. **Digital Logic**: Boolean algebra and combinational circuits (adders, subtractors)
5. **Algorithm Implementation**: Translating high-level algorithms into assembly language
6. **Memory Management**: Working with arrays and memory addresses
7. **Control Flow**: Conditional jumps, loops, and branching logic
8. **Processor Architecture**: Understanding 8085 and 8086 instruction sets and their differences

---

## 🔧 Processor Architectures Covered

- **8085 Microprocessor**: Earlier 8-bit architecture with basic instruction set
- **8086 Microprocessor**: 16-bit architecture with extended capabilities and optimized instructions

---

## 📚 How to Use This Repository

1. **Review Experiment Images**: Each PNG file contains the assembly code or circuit diagram for a specific experiment
2. **Understand Concepts**: Read the descriptions above to grasp the underlying computer architecture principles
3. **Study Implementation**: Examine the assembly code in each image to understand processor-level operations
4. **Compare Versions**: Notice differences between standard implementations and 8086-optimized versions
5. **Learn Progressively**: Start with basic arithmetic, move to complex algorithms, then to circuit theory

---

## 💡 Topics Covered

- ✅ Binary Arithmetic & Complements
- ✅ 8-bit & 16-bit Operations
- ✅ Assembly Language Programming
- ✅ Digital Logic Circuits
- ✅ Algorithm Implementation in Assembly
- ✅ Array Processing
- ✅ Mathematical Functions
- ✅ Sorting Techniques
- ✅ Processor-Specific Optimizations (8085 vs 8086)

---

## 📖 Educational Value

This repository is ideal for:
- Computer Architecture courses
- Microprocessor programming labs
- Digital logic design studies
- Low-level systems programming
- Assembly language learning
- CPU design and optimization studies

---

## 👤 Author

Created by **Saideepak1806** as a comprehensive reference for computer architecture experiments and assembly language programming.

---

## 📝 Notes

- All experiments are documented with clear implementation details
- Each experiment demonstrates a specific computer architecture concept
- Images show both the problem statement and complete assembly code solutions
- Suitable for educational purposes and reference material

---

**Last Updated**: November 2025

---

*This repository serves as a practical guide to understanding how computers work at the most fundamental level—the instruction set and digital logic that power modern processors.*
